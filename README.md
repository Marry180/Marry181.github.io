<!DOCTYPE html>
<html lang="ru">
   <head>
        <meta charset="utf-8">
        <title>Лабораторная работа 2</title>
        <link rel="stylesheet" href="style.css">
        <script>
            
            function CreateForm(){
                let button3_0 = document.createElement('input');
                button3_0.setAttribute("id", "button3_0");
                document.getElementById("div_batton").appendChild(button3_0);
                button3_0.type="button";
                button3_0.value = "Сгенерировать коофициэнты";
                button3_0.setAttribute("onclick", "GenerCooficientiKramera()");
                
                let button3_1 = document.createElement('input');
                button3_1.setAttribute("id", "button3_0");
                document.getElementById("div_batton").appendChild(button3_1);
                button3_1.type="button";
                button3_1.value = "Решение Системы";
                button3_1.setAttribute("onclick", "Reshenie()");
                
                
                ///===============СТРОКА 1 (Система +  свободый коофициент) a11, a12, a13, b1
                let input0_0 = document.createElement('input');
                input0_0.setAttribute("id", "input0_0");
                input0_0.type="input";
                input0_0.value = "0_0";
                document.getElementById("div_form_1").appendChild(input0_0);
                
                let input0_1 = document.createElement('input');
                input0_1.setAttribute("id", "input0_1");
                input0_1.type="input";
                input0_1.value = "0_1";
                document.getElementById("div_form_1").appendChild(input0_1);
                
                let input0_2 = document.createElement('input');
                input0_2.setAttribute("id", "input0_2");
                input0_2.type="input";
                input0_2.value = "0_2";
                document.getElementById("div_form_1").appendChild(input0_2);
                
                let input_b1 = document.createElement('input');
                input_b1.setAttribute("id", "input_b1");
                input_b1.type="input";
                input_b1.value = "b1";
                document.getElementById("div_form_1").appendChild(input_b1);
                //====================================================================
                
                ///===============СТРОКА 1 (Система +  свободый коофициент) a11, a12, a13, b1
                let input1_0 = document.createElement('input');
                input1_0.setAttribute("id", "input1_0");
                input1_0.type="input";
                input1_0.value = "1_0";
                document.getElementById("div_form_2").appendChild(input1_0);
                
                let input1_1 = document.createElement('input');
                input1_1.setAttribute("id", "input1_1");
                input1_1.type="input";
                input1_1.value = "1_1";
                document.getElementById("div_form_2").appendChild(input1_1);
                
                let input1_2 = document.createElement('input');
                input1_2.setAttribute("id", "input1_2");
                input1_2.type="input";
                input1_2.value = "1_2";
                document.getElementById("div_form_2").appendChild(input1_2);
                
                let input_b2 = document.createElement('input');
                input_b2.setAttribute("id", "input_b2");
                input_b2.type="input";
                input_b2.value = "b2";
                document.getElementById("div_form_2").appendChild(input_b2);
                //====================================================================
                
                ///===============СТРОКА 1 (Система +  свободый коофициент) a11, a12, a13, b1
                let input2_0 = document.createElement('input');
                input2_0.setAttribute("id", "input2_0");
                input2_0.type="input";
                input2_0.value = "2_0";
                document.getElementById("div_form_3").appendChild(input2_0);
                
                let input2_1 = document.createElement('input');
                input2_1.setAttribute("id", "input2_1");
                input2_1.type="input";
                input2_1.value = "2_1";
                document.getElementById("div_form_3").appendChild(input2_1);
                
                let input2_2 = document.createElement('input');
                input2_2.setAttribute("id", "input2_2");
                input2_2.type="input";
                input2_2.value = "2_2";
                document.getElementById("div_form_3").appendChild(input2_2);
                
                let input_b3 = document.createElement('input');
                input_b3.setAttribute("id", "input_b3");
                input_b3.type="input";
                input_b3.value = "b3";
                document.getElementById("div_form_3").appendChild(input_b3);
                //====================================================================
            }
            </script>
    </head>
    
    <body onLoad ="CreateForm()">
    <header>
        <p class="page-title"></p>
        
        <nav>
        </nav>
    
    </header>
    
    <main>
        
    </main>
    <section>
    <table cellpadding="10" border="1" width="100%">
    <tr>
        <th colspan = "4">
        <p>Создайте скрипт, выводящий на экран свойства и значения следующих объектов: window, document, location, navigator. При выполнении задания используйте оператор for ... in.</p>
        </th>
    </tr>
    
    <tr>
        <td>
            <form><button type="button" onclick="myFunctionWindow()">window</button></form>
            <textarea  id = "z3_1" rows="3" cols="45" class = "prokrutka" readonly></textarea>
        </td>
        
        <td>
            <form><button type="button" onclick="myFunctionDocument()">document</button></form>
            <textarea  id = "z3_2" rows="3" cols="45" class = "prokrutka" readonly></textarea>
        </td>
        
        <td>
            <form><button type="button" onclick="myFunctionLocation()">location</button></form>
            <textarea  id = "z3_3" rows="3" cols="45" class = "prokrutka" readonly></textarea>
        </td>
        
        <td>
            <form><button type="button" onclick="myFunctionNavigator()">navigator</button></form>
            <textarea  id = "z3_4" rows="3" cols="45" class = "prokrutka" readonly></textarea>
        </td>
    </tr>
    </table>
    </section>
    
    <p></p>
    <section>
    <table cellpadding="10" border="1" width="100%">
        <tr>
            <th id = "z4" colspan = "10">
            <p>Сгенерируйте с помощью двумерного массива и функции random() матрицу размера (10х10). Выведите ее на экран с помощью текстовых полей (сами поля, а также кнопки – обработчики событий должны создаваться при помощи скрипта). По щелчку на кнопке «Сортировка » отсортировать нечетные строки массива по возрастанию, а четные по убыванию.</p>
                
            <script>
                let parent_div = document.createElement("div");
                parent_div.id = "parent"
                let button1 = document.createElement('input');
                button1.setAttribute("id", "myBt1");
                //button1.id = "myBt1";
                button1.type="button";
                button1.value = "Генерировать массив 10х10"
                button1.setAttribute("onclick", "myKlick1()")
                z4.prepend(button1);
                
                let button2 = document.createElement('input');
                button2.setAttribute("id", "myBt2");
                //button1.id = "myBt1";
                button2.type="button";
                button2.value = "Сортировка"
                button2.setAttribute("onclick", "myKlick2()")
                myBt1.after(button2);
                
                        /*let td_z4 = document.getElementById("z4");
                        let myInput = document.createElement('input');
                        d_z4.prepend(myInput);
                        for (let i = 0; i<10; i++) {
                        	td_z4.append(myInput);
                          for (let j = 0; i<10; j++) {
                               td_z4.prepend(myInput);
                            }
                        }*/
            </script>
            </th>
        </tr>
        
        <tr id = "z4g">
            <!--<td id = "z4g">
               <!--<input>
                <tr>
                   <td>
                   
                   </td>
                </tr>
            </td>-->
        </tr>
    </table>
    </section>
    
    <p></p>
    <section>
        <table cellpadding="10" border="1" width="100%">
            <tr>
                <th onLoad ="CreateForm()"><!--onLoad ="CreateForm()"-->
                <p>Создать программу для решения системы трех линейных однородных уравнений с тремя переменными методом Крамера. Коэффициенты при переменных и свободные коэффициенты должны генерироваться автоматически (функция random() модуля Math) при щелчке по кнопке «Сгенерировать коэффициенты» и отображаться на текстовых полях. </p>
                <p>По щелчку на кнопке «Решение системы» необходимо вывести сообщение имеет ли система решение и если да, то вывести его в поля X1,X2 и X3. Расчет определителей необходимо организовать в виде функций. </p>
                <p>Поля и кнопки создать на этапе загрузки страницы (программируем события onLoad тега <body> в виде вызова функции CreateForm(), которую в свою очередь описываем в скрипте между тегами <head>).</p>
                <div id = "div_batton"></div>
                <div id = "div_form">
                    <div id = "div_form_1"> </div>
                    <div id = "div_form_2"> </div>
                    <div id = "div_form_3"> </div>
                </div>
                
                </th>
            </tr>
        </table>
    </section>
    
    <footer>
    </footer>
    <script src="JavaScript.js"></script>
    </body>
    
</html>
