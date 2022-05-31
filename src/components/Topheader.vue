<template>
    <div id="toHeader">
        <nav>
            <div class="logo">
                <span>
                    <strong>
                        <a href="#">{{logo}}</a>
                    </strong>
                </span>
            </div>
            <div class="lang">
                <span style="color: #469d6e">{{banglaLanguage}}</span>
                /
                <span>{{englishLanguage}}</span>
            </div>
        </nav>
    </div>
</template>
<script>
export default {
    name: 'Topheader',
    data() {
        return {
            logo: 'LOGO',
            banglaLanguage: 'BN',
            englishLanguage: 'EN'
        }
    }
}
</script>
<style lang="scss" scoped>
nav {
    display: flex;
    justify-content: space-between;
    padding: 20px;
    align-items: center;
    a{
        text-decoration: none;
        color: #404040;
        font-size: 25px;
    }
}
</style>
