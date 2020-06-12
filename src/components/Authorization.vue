<template>
    <body @submit.prevent="onSubmit">
    <div class="limiter">
        <div class="container-login100">
            <div class="wrap-login100 p-t-85 p-b-20">
                <form class="login100-form validate-form">
					<span class="login100-form-title p-b-70">
						Welcome
					</span>

                    <div class="wrap-input100 validate-input m-t-85 m-b-35" data-validate = "Enter username">
                        <input class="input100" type="text" name="username" v-model="login">
                        <span class="focus-input100" data-placeholder="Username"></span>
                    </div>

                    <div class="wrap-input100 validate-input m-b-50" data-validate="Enter password">
                        <input class="input100" type="password" name="pass" v-model="password">
                        <span class="focus-input100" data-placeholder="Password"></span>
                    </div>

                    <div class="container-login100-form-btn">
                        <button class="login100-form-btn" type="submit">
                            Login
                        </button>
                    </div>

                </form>
            </div>
        </div>
    </div>
    <div id="dropDownSelect1"></div>
    </body>
</template>

<script>
    export default {
        name: "Authorization",
        data(){
           return{ login: '',
                password: ''
           }
        },
        mounted(){
            fetch('http://localhost:8080/login')
        },
        methods:{
            onSubmit(){
                console.log(this.login)
                console.log(this.password)


            }
        }
    }
</script>




<style scoped>

</style>