<template>
    <footer>
        <div class="row">
                <div class="col-md-3">
                    <ul>
                        <li class="my-3">
                            <a href="#">
                                We are social
                            </a>
                        </li>
                        <li class="my-3">
                            <a href="#">
                                FOLLOW US
                            </a>
                        </li>
                        <li class="my-3">
                            <a href="#">
                                <i class="fab fa-instagram-square fa-2x mx-2" style="color: #F56040;"></i>
                                <i class="fab fa-facebook fa-2x mx-2" style="color: #4267B2;"></i>
                                <i class="fab fa-youtube-square fa-2x mx-2" style="color: #FF0000;"></i>
                            </a>
                        </li>
                        <li class="my-4">
                            <a href="#" class="fw">
                                <strong>
                                    <b>
                                        LOGO
                                    </b>
                                </strong>
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <ul>
                        <li v-for="link in links" :key="link" class="my-3">
                            <a href="#">
                                <strong>
                                    {{link}}
                                </strong>
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <ul>
                        <li v-for="documentation in documentations" :key="documentation" class="my-3">
                            <a href="#">
                                <strong>
                                    {{documentation}}
                                </strong>
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <ul>
                        <li v-for="support in supports" :key="support" class="my-3">
                            <a href="#">
                                {{support}}
                            </a>
                        </li>
                    </ul>
                </div>
        </div>
    </footer>
</template>
<script>
export default {
    name: 'Footer',
    data() {
        return {
            links: [
                'Links',
                'ADVERTISERS FAQ',
                'PUBLISHERS',
                'INFLUENCERS',
                'AD FORMATS'
            ],
            documentations: [
                'Documentation',
                'TERMS & CONDITIONS',
                'PRIVACY POLICY',
                'CANCELLATION POLICY',
                'BLOG',
            ],
            supports: [
                'Support',
                'FAQ',
                'FOLLOW US',
                'MEDIA KIT',
                'CONTACT US',
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
footer {
    margin-top: 80px;
    ul li {
        list-style-type: none;
        a{
            text-decoration: none;
            color: #404040;
        }
        .fw{
            font-size: 25px;
        }
    }
}
</style>
