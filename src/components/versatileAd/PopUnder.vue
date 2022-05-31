<template>
    <div class="popUnderContent">
        <div class="popUnderImg">
            <img src="../../assets/popUnder.jpg" alt="">
        </div>
        <div class="popUnderText">
                <h5>
                    {{popUnder[0].title}}
                </h5>
                <p>
                    {{popUnder[0].text}}
                </p>
                <a href="#">
                    {{popUnder[0].link}} 
                     <i class="fas fa-external-link mx-1"></i>
                </a>
        </div>
    </div>
</template>
<script>
export default {
    name: 'PopUnder',
    data() {
        return {
            popUnder: [
                {
                    title: 'POP-UNDER',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, minus quis! Expedita, mollitia. Neque, impedit.',
                    link: 'Learn more'
                }
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
.popUnderContent{
    display: flex;
    justify-content: space-between;
    text-align: center;
    flex-wrap: wrap;
    height: 300px;
    margin-top: 40px;
    .popUnderImg img{
        width: 400px;
        height: 250px;
    }
    .popUnderText{
        width: 500px;
        h5{
            color: #FF6F00;
        }
        a{
            color: #644F9C;
        }
    }
}
</style>
