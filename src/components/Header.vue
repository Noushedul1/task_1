<template>
    <div class="navItem">
        <nav class="navbar navbar-expand-lg navbar-light">
            <div class="container-fluid">
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav">
                    <li class="nav-item" v-for="navItem in navItems" :key="navItem">
                    <a class="nav-link" aria-current="page" href="#">
                        {{navItem}}
                    </a>
                    </li>
                </ul>
                </div>
                <div class="loginAndSignup">
                    <button class="login">
                        <a href="#">
                            LOGIN
                        </a>
                    </button>
                    <button class="signUp">
                        <a href="#">
                            SIGN UP
                        </a>
                    </button>
                </div>
            </div>
        </nav>
    </div>
</template>
<script>
export default {
    name: 'Header',
    data() {
        return {
            navItems: [
                'HOME',
                'ADVERTISERS',
                'PUBLISHERS',
                'INFLUENCERS',
                'AD FORMATS',
                'BLOG',
                'CONTACT US '
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
nav ul li a{
    color: #644F9C !important;
    &:active{
        color: #FF6F00 !important;
    }
}
.loginAndSignup{
    position: relative;
    right: 60px;
    .login{
        border: none;
        display: block;
        padding: 15px 140px 15px 15px;
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;
        border-bottom-left-radius: 10px;
        border-bottom-right-radius: 10px;
        background: white;
        box-shadow: -1px 1px 10px -3px grey;
        a{
            text-decoration: none;
            color: #404040;
        }
    }
    .signUp{
        @extend .login;
        position: absolute;
        background: #FF6F00;
        padding: 5px 40px 5px 10px;
        bottom: 10px;
        left: 70px;
        color: white;
        a{
            text-decoration: none;
            color: #F2F2F2;
        }
    }
}
</style>
