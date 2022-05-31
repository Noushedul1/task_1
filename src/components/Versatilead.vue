<template>
    <div class="versatile">
        <div>
            <h4 class="text-center">
                {{versatile}}
            </h4>
        </div>
        <div class="versatileBtnContent">
            <div class="btnContent">
                <button @click="versatileComp='PopUnder'" class="my-2">Pop Under</button>
                <button @click="versatileComp='Banner'" class="my-2">Banner Ad</button>
                <button @click="versatileComp='Native'" class="my-2">Native</button>
                <button @click="versatileComp='Skim'" class="my-2">Skim</button>
            </div>
            <component :is="versatileComp"></component>
        </div>
    </div>
</template>
<script>
import PopUnder from '../components/versatileAd/PopUnder.vue';
import Banner from '../components/versatileAd/BannerAd.vue';
import Native from '../components/versatileAd/Native.vue';
import Skim from '../components/versatileAd/Skim.vue';
export default {
    name: 'Versatile',
    components: {
        PopUnder,
        Banner,
        Native,
        Skim
    },
    data() {
        return {
            versatile: 'VERSATILE AD FORMATS',
            versatileComp: 'PopUnder'
        }
    }
}
</script>
<style lang="scss" scoped>
.versatile{
    margin-top: 30px;
     h4{
        color: #644F9C;
        position: relative;
    }
    h4::before{
        content: "";
        display: block;
        width: 35%;
        border-width: 1px;
        border-style: dotted;
        left: 0;
        top: 50%;
        position: absolute;
        color: black;
    }
       h4::after{
        content: "";
        display: block;
        width: 35%;
        border-width: 1px;
        border-style: dotted;
        position: absolute;
        right: 0;
        top: 50%;
        color: black;
    }
    .versatileBtnContent{
        text-align: center;
        margin-top: 30px;
        .btnContent{
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            button{
                border: none;
                padding: 5px 40px;
                border-start-end-radius: 10px;
                border-end-end-radius: 10px;
                border-bottom-left-radius: 10px;
                border-top-left-radius: 10px;
                box-shadow: -1px 5px 10px -3px grey;
                transition: all .6s ease-in;
                &:hover{
                    background: #FF6F00;
                    color: #F2F2F2;
                }
            }
        }
    }
     @media (max-width: 768px){
        h4::before,
        h4::after{
            width: 18%;
        }
    }
    @media (max-width: 1100px){
        h4::before,
        h4::after{
            width: 23%;
        }
    }
}
</style>
