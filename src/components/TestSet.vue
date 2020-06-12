<template>
    <div id="testSetDiv" style="margin-left: 20px">
        <h1>{{setName}}</h1>
        <hr>
        <br>
        <h3>Описание</h3>
        <p style="font-size: 20px">Данный набор тестовых сценариев содержит проверки авторизации
            пользователя</p>
        <hr>
        <br>
        <span style="font-size: 24px">Тестирование: </span>
        <span style="font-size: 24px; color: #006666;" >Ручное</span>

        <br><br>
        <ul class="hr">
            <li><a href>Test-case 1. Авторизация. Отправка запроса login</a></li>
            <li><a href>Test-case 2. Авторизация. Положительный сценарий</a></li>
            <li><a href>Test-case 3. Авторизация. Ошибочные сценарии</a></li>

        </ul>
    </div>
</template>

<script>
    export default {
        name: "TestSet",
        props: {
            setName: String
        }
    }
</script>

<style scoped>

    p{
        font-family: 'Arial'
    }
    span {
        font-family: 'Arial'
    }

    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background: linear-gradient(to bottom, #006666, #FFFFFF);
        /* background-color: #009999;*/
    }

    ul.hr {
        margin-left: 20px;
        margin-right: 30px;
        padding: 4px; /* Значение полей */

    }

    ul.hr li {
        padding: 3px; /* Поля вокруг текста */

        font-size: 30px;
        color: #ffffff;
    }

    A {

        font-size: 20px;
        color: #006666;
        line-height: 1.2;
    }

    A:hover {
        color: #062626;
    }

    A:active {
        color: #010909;
    }


</style>