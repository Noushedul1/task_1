<template>
    <div class="bannerContent">
        <div class="bannerImg">
            <img src="../../assets/banner2.jpg" alt="">
        </div>
        <div class="bannerText">
                <h5>
                    {{banner[0].title}}
                </h5>
                <p>
                    {{banner[0].text}}
                </p>
                <a href="#">
                    {{banner[0].link}} 
                     <i class="fas fa-external-link mx-1"></i>
                </a>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Banner',
    data() {
        return {
            banner: [
                {
                    title: 'BANNER',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, minus quis! Expedita, mollitia. Neque, impedit.',
                    link: 'Learn more'
                }
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
.bannerContent{
    display: flex;
    justify-content: space-between;
    text-align: center;
    flex-wrap: wrap;
    height: 300px;
    margin-top: 40px;
    .bannerImg img{
        width: 400px;
        height: 250px;
    }
    .bannerText{
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
