<template>
    <div class="skimContent">
        <div class="skimImg">
            <img src="../../assets/skim.jpg" alt="">
        </div>
        <div class="skimText">
                <h5>
                    {{skim[0].title}}
                </h5>
                <p>
                    {{skim[0].text}}
                </p>
                <a href="#">
                    {{skim[0].link}} 
                     <i class="fas fa-external-link mx-1"></i>
                </a>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Skim',
    data() {
        return {
            skim: [
                {
                    title: 'SKIM',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, minus quis! Expedita, mollitia. Neque, impedit.',
                    link: 'Learn more'
                }
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
.skimContent{
    display: flex;
    justify-content: space-between;
    text-align: center;
    flex-wrap: wrap;
    height: 300px;
    margin-top: 40px;
    .skimImg img{
        width: 400px;
        height: 250px;
    }
    .skimText{
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
