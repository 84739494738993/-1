<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
     <!-- <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/84739494738993/proba/x.css"> -->
     <link rel="stylesheet" href="x.css">

    


</head>
<body>
    <div>
        <div id="login-form" class="container1">
            <h2>Вход</h2>
            <input type="text" id="username" placeholder="Имя пользователя">
            <input type="password" id="password" placeholder="Пароль">
            <button id="login-button">Войти</button>
            

        </div>
    </div>
    <div id="all">
        <div class="number"  id="number1">
            <input type="button" value="Вопрос:1">
            <p class="question"> Что такое закон сохранения энергии?</p>
            <input type="text" class="answer" id="answer1" placeholder="ОТВЕТ">
        </div>
        <div class="number"id="number2" >
            <input type="button" value="Вопрос:2">
            <p class="question">Основные формы энергии?</p>
            <input type="text" class="answer" id="answer2" placeholder="ОТВЕТ">
        </div>
        <div class="number"id="number3">
            <input type="button" value="Вопрос:3">
            <p class="question">Единица измерения силы?</p>
            <input type="text" class="answer" id="answer3" placeholder="ОТВЕТ">
        </div>
        <div class="number"id="number4">
            <input type="button" value="Вопрос:4">
            <p class="question">Скорость света в вакууме?</p>
            <input type="text" class="answer" id="answer4" placeholder="ОТВЕТ">
        </div>
        <div class="number"id="number5">
            <input type="button" value="Вопрос:5">
            <p class="question">Частицы, составляющие атом?</p>
            <input type="text" class="answer" id="answer5" placeholder="ОТВЕТ">
        </div>
        <div class="number"id="number6">
            <input type="button" value="Вопрос:6">
            <p class="question">Единица измерения электрического заряда?</p>
            <input type="text" class="answer" id="answer6" placeholder="ОТВЕТ">
        </div>
        <div class="number"id="number7">
            <input type="button" value="Вопрос:7">
            <p class="question"> Уравнение Эйнштейна, описывающее отношение массы и энергии?</p>
            <input type="text" class="answer" id="answer7" placeholder="ОТВЕТ">
        </div>
        <div class="number" id="number8">
            <input type="button" value="Вопрос:8">
            <p class="question">Закон сохранения импульса?</p>
            <input type="text" class="answer" id="answer8" placeholder="ОТВЕТ">
        </div>
        <div class="number" id="number9">
            <input type="button" value="Вопрос:9">
            <p class="question"> Самая сильная из известных фундаментальных сил природы?</p>
            <input type="text" class="answer" id="answer9" placeholder="ОТВЕТ">
        </div>
        <div class="number" id="number10">
            <input type="button" value="Вопрос:10">
            <p class="question"> Единица измерения энергии?</p>
            <input type="text" class="answer" id="answer10" placeholder="ОТВЕТ">
    </div>
    <input type="hidden" class="correct-answer" value="correct answer2">
</div>
<div><input type="button" value="ПРОВЕРИТЬ" id="check"></div>
<div id="result">Счет:0</div>
<button id="clean">Очистить данние таблици</button>
</div>
<!-- <script src="https://cdn.jsdelivr.net/gh/84739494738993/proba/x.js"></script> -->
<script src="x.js"></script>

<style>@media only screen and (max-width: 600px) {
    /* Ваши стили для маленьких экранов */
}
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.container1 {
    width: 300px;
    margin: auto;
    background-color: #fff;
    border-radius: 5px;
    padding: 20px;
    box-shadow: 0px 0px 10px 0px rgba(0,0,0,0.1);
}


input[type="text"],
input[type="password"],
select,
textarea {
    width: calc(100% - 20px);
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #ccc;
    border-radius: 3px;
}

button{
    width: 100%;
    padding: 10px;
    background-color: #4caf50;
    color: #fff;
    border: none;
    border-radius: 3px;
    cursor: pointer;
}


#clean{
    width: 200px;
    height: 60px;
    display: none;
    position: relative;
    position: fixed;
    top: 25px;
    left:1300px;
}

/* button:hover {
    background-color: #45a049;
} */

#errorMsg {
    color: red;
    font-size: 0.8em;
    margin-top: 5px;
}

#teacherMenu,
#studentMenu {
    display: none;
}

#all {
    display: none;
    width: 100vw;
    height: 100vh; 
}

.number input[type="button"] {
    display: block; /* Делаем кнопки блочными, чтобы они располагались друг под другом */
    margin-bottom: 15px; /* Добавляем небольшой отступ между кнопками */
}



.question,
.answer {
    display: none; 
    position: relative;
    left: 400px;

}

input[type="button"] {
    margin-top: 40px;
    margin-left: 150px;
    width: 150px;
    height: 40px;
    font-size: 16px;
    color:  rgb(255, 255, 255);
    background-color: rgb(100, 100, 100);
}
/* input[type="button"]:hover {
background-color:rgb(255, 255, 255);
color:  rgb(100, 100, 100);
} */

#check {
    width: 300px;
    height: 100px;
    position: relative;
    top: 600px;
    left: -550px;
    background-color: #45a049;
    color: #ffffff;
    display: none;
    
}

#result{
    width: 200px;
    height: 60px;
    position: relative;
    position: fixed;
    top: 25px;
    left: 1300px;
    background-color: red;
    color: #ffffff;
    font-size: 50px;
    text-align: center;
    display: none;
}
</style>

<script>// Сохраняем и проверяем имя пользователя и пароль
    // const savedUsername = ["user", "a","ф"];
    // const savedPassword = ["password", "a", "ф"];
    let a = 0;
    
    
    // Функция для проверки введенных данных
    // function checkCredentials(username, password) {
    //     return savedUsername.includes(username) && savedPassword.includes(password);
    // }
    function tablica() {
        // Получаем таблицу по ее идентификатору
        const table = document.getElementById("scoreTable");
        table.style.display = "none";
    }
    
    // Функция для обработки попытки входа
        function login() {
            const usernameInput = document.getElementById("username");
            const passwordInput = document.getElementById("password");
            const username = usernameInput.value;
            const password = passwordInput.value;
    
            // if (checkCredentials(username, password)) {
            //     // Если данные верные, показываем контейнер для теста и скрываем форму входа
            //     document.getElementById("login-form").style.display = "none";
            //     document.getElementById("all").style.display = "block";
            //     document.getElementById("check").style.display = "block";
            //     // Проверяем ответы на вопросы
            //     checkAnswers();
    
            // }
                if (username === "Людмила" && password === "3568") {
                    score();
                    // Обновляем таблицу
                    updateTable(JSON.parse(localStorage.getItem("userData")));
                    document.getElementById("login-form").style.display = "none";
                    document.getElementById("all").style.display = "none";
                    document.getElementById("check").style.display = "none";
                    document.getElementById("clean").style.display = "block";
       
                }
            else {
            document.getElementById("login-form").style.display = "none";
            document.getElementById("all").style.display = "block";
            document.getElementById("check").style.display = "block";
            checkAnswers();
        
            }
        }
        function clean(){
        // очистка
        localStorage.removeItem("userData");
        alert("Очистка била проведена.");
    
        }
    
    // Привязываем функцию к кнопке входа
    document.getElementById("login-button").addEventListener("click", login);
    document.getElementById("clean").addEventListener("click", clean);
    
    function checkAnswers() {
        // Проходим по всем элементам с классом "number"
        const numberElements = document.querySelectorAll('.number');
        numberElements.forEach((numberElement, index) => {
            // Получаем кнопку внутри текущего элемента
            const button = numberElement.querySelector('input[type="button"]');
            // Получаем соответствующий элемент вопроса и ответа
            const question = numberElement.querySelector('.question');
            const answer = numberElement.querySelector('.answer');
            // Привязываем обработчик события к кнопке
            button.addEventListener('click', function() {
                // Скрываем остальные вопросы и ответы
                numberElements.forEach((element) => {
                    if (element !== numberElement) {
                        element.querySelector('.question').style.display = 'none';
                        element.querySelector('.answer').style.display = 'none';
                        
                    }
                });
                // Показываем текущий вопрос и ответ
                question.style.display = 'block';
                answer.style.display = 'block';
                if (a>0){
                    question.style.display = 'none';
                    answer.style.display = 'none';
                }
            });
        });
    }
    
    const questionButton1 = document.querySelector('input[value="Вопрос:1"]');
    const questionButton2 = document.querySelector('input[value="Вопрос:2"]');
    const questionButton3 = document.querySelector('input[value="Вопрос:3"]');
    const questionButton4 = document.querySelector('input[value="Вопрос:4"]');
    const questionButton5 = document.querySelector('input[value="Вопрос:5"]');
    const questionButton6 = document.querySelector('input[value="Вопрос:6"]');
    const questionButton7 = document.querySelector('input[value="Вопрос:7"]');
    const questionButton8 = document.querySelector('input[value="Вопрос:8"]');
    const questionButton9 = document.querySelector('input[value="Вопрос:9"]');
    const questionButton10 = document.querySelector('input[value="Вопрос:10"]');
    
    const answerField1 = document.getElementById('answer1');
    const answerField2 = document.getElementById('answer2');
    const answerField3 = document.getElementById('answer3');
    const answerField4 = document.getElementById('answer4');
    const answerField5 = document.getElementById('answer5');
    const answerField6 = document.getElementById('answer6');
    const answerField7 = document.getElementById('answer7');
    const answerField8 = document.getElementById('answer8');
    const answerField9 = document.getElementById('answer9');
    const answerField10 = document.getElementById('answer10');
    
    const answerFields = [
        document.getElementById('answer1'),
        document.getElementById('answer2'),
        document.getElementById('answer3'),
        document.getElementById('answer4'),
        document.getElementById('answer5'),
        document.getElementById('answer6'),
        document.getElementById('answer7'),
        document.getElementById('answer8'),
        document.getElementById('answer9'),
        document.getElementById('answer10')
    ];
    
    let result = 0;
    
    function Answer() {
        // if(answerField1.value > "" && answerField2.value > "" && answerField2.value > "" && answerField3.value > "" && answerField4.value > "" && answerField5.value > "",answerField6.value > ""  && answerField7.value > ""  && answerField8.value > "" && answerField9.value > "" && answerField10.value > ""){
            
            var answer1 = answerField1.value.toLowerCase();
            var answer2 = answerField2.value.toLowerCase();
            var answer3 = answerField3.value.toLowerCase();
            var answer4 = answerField4.value.toLowerCase();
            var answer5 = answerField5.value.toLowerCase();
            var answer6 = answerField6.value.toLowerCase();
            var answer7 = answerField7.value.toLowerCase();
            var answer8 = answerField8.value.toLowerCase();
            var answer9 = answerField9.value.toLowerCase();
            var answer10 = answerField10.value.toLowerCase();
    
            if (answer1 === "сумма") {
            a += 1;
            questionButton1.style.backgroundColor = "green";
            result++;
        } else {
            questionButton1.style.backgroundColor = "red";
        }
    
        if (answer2 === "кинетическая") {
            a += 1;
            questionButton2.style.backgroundColor = "green";
            result++;
        } else {
            questionButton2.style.backgroundColor = "red";
        }
    
        if (answer3 === "ньютон") {
            a += 1;
            questionButton3.style.backgroundColor = "green";
            result++;
        } else {
            questionButton3.style.backgroundColor = "red";
        }
    
        if (answer4 === "константа") {
            a += 1;
            questionButton4.style.backgroundColor = "green";
            result++;
        } else {
            questionButton4.style.backgroundColor = "red";
        }
    
        if (answer5 === "протоны") {
            a += 1;
            questionButton5.style.backgroundColor = "green";
            result++;
        } else {
            questionButton5.style.backgroundColor = "red";
        }
    
        if (answer6 === "кулон") {
            a += 1;
            questionButton6.style.backgroundColor = "green";
            result++;
        } else {
            questionButton6.style.backgroundColor = "red";
        }
    
        if (answer7 === " e=mc²") {
            a += 1;
            questionButton7.style.backgroundColor = "green";
            result++;
        } else {
            questionButton7.style.backgroundColor = "red";
        }
    
        if (answer8 === "инерция") {
            a += 1;
            questionButton8.style.backgroundColor = "green";
            result++;
        } else {
            questionButton8.style.backgroundColor = "red";
        }
    
        if (answer9 === "сила") {
            a += 1;
            questionButton9.style.backgroundColor = "green";
            result++;
        } else {
            questionButton9.style.backgroundColor = "red"; 
        }
            if(answerField10.value === "джоуль"){
                a+=1
                questionButton10.style.backgroundColor = "green";
                result++
                score();
            }
            else{
                questionButton10.style.backgroundColor = "red";
                    score(); // вызываем функцию score() только если ответы на все вопросы были проверены
                }
            }
        
    //     else{
    //         alert("Вы не ввели везде ответы!");
    //     }
    // }
    
    // Ваш код здесь
    
    document.getElementById("check").addEventListener("click", function() {
        // Вызываем функцию проверки ответов
        Answer();
        // Вызываем функцию для скрытия таблицы и вывода сообщения об ошибке
        tablica();
        // Очищаем таблицу
        clearTable();
    });
       
    function score() {
        a += 1;
        document.getElementById("result").style.display = "block";
        const resultElement = document.getElementById("result");
        resultElement.textContent = "Счет:" + result;
        document.getElementById("check").style.display = "none";
        // document.getElementById("scoreTable").style.display = "block";
    
        // Вызываем функцию updateTable() после загрузки DOM
        document.addEventListener("DOMContentLoaded", function() {
            var savedData = localStorage.getItem("userData");
            if (savedData) {
                var userData = JSON.parse(savedData);
                updateTable(userData);
            }
        });
    
        // Получаем имя пользователя
        var username = document.getElementById("username").value;
    
        // Создаем или получаем данные из Local Storage
        var savedData = localStorage.getItem("userData");
        var userData = savedData ? JSON.parse(savedData) : [];
    
        // Добавляем данные текущего пользователя
        var userAnswers = [];
        for (var j = 1; j <= 10; j++) {
            var answerField = document.getElementById("answer" + j); 
            userAnswers.push(answerField.value);
        }
        userData.push({ username: username, answers: userAnswers });
    
        // Сохраняем данные в Local Storage
        localStorage.setItem("userData", JSON.stringify(userData));
    
        // Обновляем таблицу
        updateTable(userData);
    }
    
    function updateTable(userData) {
        // Очищаем таблицу
        var table = document.getElementById("scoreTable");
        if (table) {
            table.parentNode.removeChild(table);
        }
    
        // Создаем новую таблицу
        table = document.createElement("table");
        table.setAttribute("border", "5px");
        table.setAttribute("id", "scoreTable");
    
        // Устанавливаем стиль display для скрытия таблицы
        // table.style.display = "none";
    
        // Создаем заголовок таблицы
        var thead = document.createElement("thead");
        var headerRow = document.createElement("tr");
        var idHeader = document.createElement("th");
        idHeader.textContent = "Имя пользователя";
        headerRow.appendChild(idHeader);
    
        // Создаем столбцы для каждого элемента answerField
        for (var i = 1; i <= 10; i++) {
            var columnHeader = document.createElement("th");
            columnHeader.textContent = "Ответ " + i;
            headerRow.appendChild(columnHeader);
        }
    
        thead.appendChild(headerRow);
        table.appendChild(thead);
    
        // Создаем тело таблицы
        var tbody = document.createElement("tbody");
    
        // Добавляем данные каждого пользователя в таблицу
        userData.forEach(function(user) {
            var userRow = document.createElement("tr");
            var userCell = document.createElement("td");
            userCell.textContent = user.username;
            userRow.appendChild(userCell);
    
            user.answers.forEach(function(answer) {
                var answerCell = document.createElement("td");
                answerCell.textContent = answer;
                userRow.appendChild(answerCell);
            });
    
            tbody.appendChild(userRow);
        });
    
        table.appendChild(tbody);
    
        document.body.appendChild(table);
    }</script>


</body>
</html>

