<template>

    <header >
        <div class="header-left"> <img src="../assets/logo.png" alt="logo" style="margin-left: 20px" > </div>
        <div align="left">
            <ul class="hr">
                <li> <a href=""> about project </a> </li>
                <li> <a href=""> test model </a> </li>
                <li> <a href=""> create </a> </li>
                <li> <a href=""> home </a> </li>
            </ul>
        </div>

    </header>

</template>

<script>
    export default {
        name: "HeaderAuthorized"
    }
</script>

<style scoped>
    header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        background: linear-gradient(to bottom, #006666, #FFFFFF) ;
        /* background-color: #009999;*/
    }
    ul.hr{
        margin: 0; /* Обнуляем значение отступов */
        padding: 4px; /* Значение полей */
        text-align: left;

    }
    ul.hr li{
        display: inline; /* Отображать как строчный элемент */
        padding: 3px; /* Поля вокруг текста */
        font-family: Poppins-Medium;
        font-size: 50px;
        color: #ffffff;
        text-transform: uppercase;

    }
    A {
        font-family: Poppins-Medium;
        font-size: 20px;
        color: #006666;
        line-height: 1.2;
        text-transform: uppercase;
    }
    A:hover{
        color: #062626;
    }
    A:active {
        color: #010909;
    }


</style>