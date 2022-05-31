<template>
    <div class="banner">
        <div class="bannerTitle">
            <h1>Welcome to our AD Service</h1>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, molestias iure veniam cumque culpa aperiam laudantium unde, doloribus, enim non sapiente esse amet ipsa odit quibusdam aliquam tempora corrupti voluptatem.
            </p>
        </div>
        <div class="bannerImg">
            <img src="../assets/banner.jpg" alt="">
        </div>
    </div>
</template>
<script>
export default {
    name: 'Banner',
    data() {
        return {
            
        }
    }
}
</script>
<style lang="scss" scoped>
.banner{
    display: flex;
    margin-top: 15px;
     .bannerTitle{
        padding-top: 15px;
        p{
            padding-top: 15px;
        }
    }
    .bannerImg img{
        width: 100%;
        height: auto;
    }
}
@media (max-width: 769px) {
    .banner{
        flex-wrap: wrap;
    }
}
</style>
