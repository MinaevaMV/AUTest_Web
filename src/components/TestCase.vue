<template>
    <div id="testCaseDiv1">
        <h3>{{caseName}}</h3>
    </div>
</template>

<script>
    export default {
        name: "TestCase",
        props:{
            caseName: String
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