<template>
    <body>
    <div class="limiter" id="authorizationDiv">
        <div class="container-login100">
            <div class="wrap-login100 p-t-85 p-b-20">

					<span class="login100-form-title p-b-70">
						Welcome
					</span>
                <div class="wrap-input100 validate-input m-t-85 m-b-35" data-validate="Enter username">
                    <input class="input100" type="text" name="username" v-model="login">
                    <span class="focus-input100" data-placeholder="Username"></span>
                </div>
                <div class="wrap-input100 validate-input m-b-50" data-validate="Enter password">
                    <input class="input100" type="password" name="pass" v-model="password">
                    <span class="focus-input100" data-placeholder="Password"></span>
                </div>
                <div class="container-login100-form-btn">
                    <button class="login100-form-btn" type="submit" v-on:click="onSubmit">
                        Login
                    </button>
                </div>
            </div>
        </div>
    </div>
    <div id="dropDownSelect1"></div>
    </body>
</template>

<script>
    export default {
        name: "Authorization",
        data() {
            return {
                login: '',
                password: ''
            }
        },
        methods: {
            onSubmit() {
                console.log(this.login)
                console.log(this.password)
                this.$http.post(
                    "http://localhost:8080/rest/login", {
                        login: this.login,
                        password: this.password
                    }
                ).then(response => {
                    console.log(response);
                    document.getElementById("authorizationDiv").style.display = "none";
                    document.getElementById("aboutProjectDiv").style.display = "block";
                    document.getElementById("nonAuthorizedHeader").style.display = "none";
                    document.getElementById("authorizedHeader").style.display = "-webkit-box";
                })

            }
        }
    }
</script>


<style scoped>

</style>