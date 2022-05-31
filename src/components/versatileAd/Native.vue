<template>
    <div class="nativeContent">
        <div class="nativeImg">
            <img src="../../assets/native.jpg" alt="">
        </div>
        <div class="nativeText">
                <h5>
                    {{native[0].title}}
                </h5>
                <p>
                    {{native[0].text}}
                </p>
                <a href="#">
                    {{native[0].link}} 
                     <i class="fas fa-external-link mx-1"></i>
                </a>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Natice',
    data() {
        return {
            native: [
                {
                    title: 'NATIVE',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, minus quis! Expedita, mollitia. Neque, impedit.',
                    link: 'Learn more'
                }
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
.nativeContent{
    display: flex;
    justify-content: space-between;
    text-align: center;
    flex-wrap: wrap;
    height: 300px;
    margin-top: 40px;
    .nativeImg img{
        width: 400px;
        height: 250px;
    }
    .nativeText{
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
