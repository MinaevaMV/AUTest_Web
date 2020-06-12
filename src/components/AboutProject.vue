<template>
    <div id="aboutProjectDiv" style="margin-left: 20px" >
        <br><br>
        <h1><b>{{projectName}}</b></h1>
        <hr>
        <br>

        <div style="margin-right: 20px">
            <p style="font-size: 20px; font-family: 'Arial'" align="justify"> Autest — это семейство продуктов,
                призванных помочь самым разным командам в организации работы. Autest
                предлагает ряд продуктов и вариантов развертывания, специально разработанных для команд разработчиков
                ПО,
                ИТ-команд, бизнес-команд, операционных команд и т. д. Информация, приведенная ниже, поможет сделать
                правильный выбор.</p>
            <p style="font-size: 20px; font-family: 'Arial'" align="justify">С помощью продуктов и приложений, созданных
                на платформе Autest, команды могут планировать, назначать и
                отслеживать работу, управлять ею и создавать отчеты. На платформе Autest можно вместе заниматься чем
                угодно:
                от разработки ПО и поддержки клиентов по методике agile до работы со списками покупок и распределения
                семейных обязанностей.

                На платформе Autest созданы три продукта: Autest Software, Autest Service Desk и Autest Core. Каждый
                продукт
                включает в себя шаблоны для различных сценариев использования и органично работает в связке с другими
                продуктами, поэтому разные команды в организации могут эффективно работать вместе.</p>
        </div>
        <div>
            <br><br><br>
            <h3 style="font-size: 26px">Активности по проекту {{projectName}}</h3>
            <hr>
            <ul class="hr">
                <li v-on:click="goToSet"><p class="A">Test-set 1. Авторизация</p></li>
                <li><p class="A">Test-set 2. Регистрация</p></li>
                <li><p class="A">Test-set 3. Получение справочных данных</p></li>
                <li><p class="A">Test-set 4. Валидация параметров ответа</p></li>
                <li><p class="A">Test-set 5. Таб-бар</p></li>
                <li><p class="A">Test-set 6. Дашборд</p></li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "AboutProject",
        props: {
            projectName: String
        },
        methods:{
            goToSet(){
                document.getElementById("aboutProjectDiv").style.display = "none";
                document.getElementById("testSetDiv").style.display = "block";
            }
        }
    }
</script>

<style scoped>


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

    .A {

        font-size: 20px;
        color: #006666;
        line-height: 1.2;
    }

    .A:hover {
        color: #062626;
    }

    .A:active {
        color: #010909;
    }


</style>