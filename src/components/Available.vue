<template>
    <div class="available">
       <h4 class="text-center">
          AVAILABLE FOR EVERYONE
       </h4>
       <p class="text-center">
           Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolorem, dolores?
       </p>
       <div class="row">
           <div class="col-md-3 offset-1 my-2">
               <div class="icons">
                    <div class="box">
                        <div v-html="icons[0]" class="insideIcon"></div>
                    </div>
                    <p>
                        {{text[0]}}
                    </p>
                </div>
                <button>{{btn[0]}}</button>
           </div>
           <div class="col-md-3 offset-1 my-2">
               <div class="icons">
                    <div class="box">
                        <div v-html="icons[1]" class="insideIcon"></div>
                    </div>
                    <p>
                        {{text[1]}}
                    </p>
                </div>
                <button>{{btn[1]}}</button>
           </div>
           <div class="col-md-3 offset-1 my-2">
               <div class="icons">
                    <div class="box">
                        <div v-html="icons[2]" class="insideIcon"></div>
                    </div>
                    <p>
                        {{text[2]}}
                    </p>
                </div>
                <button>{{btn[2]}}</button>
           </div>
       </div>
    </div>
</template>
<script>
export default {
    name: 'Available',
    data() {
        return {
            icons: [
                '<i class="fas fa-bullhorn fa-4x"></i>',
                '<i class="fas fa-paper-plane fa-4x"></i>',
                '<i class="fas fa-broadcast-tower fa-4x"></i>'
            ],
            text: [
                'Text 1', 'Text 3', 'Text 4'
            ],
            btn: ['Hello 1', 'Hello 2', 'Hello 3']
        }
    }
}
</script>
<style lang="scss" scoped>
.available {
    margin-top: 15px;
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
    @media (max-width: 991px){
        h4::after{
            width: 10em;
        }
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
    button {
        border: none;
        padding: 5px 40px;
        border-start-end-radius: 10px;
        border-end-end-radius: 10px;
        border-bottom-left-radius: 10px;
        border-top-left-radius: 10px;
        background: #644F9C;
        color: #F2F2F2;
    }
    .box{
        height: 150px;
        width: 150px;
        background: rgb(241, 202, 202);
        border-radius: 50%;
        position: relative;
        text-align: center;
        .insideIcon{
            position: absolute;
            top: 30%;
            left: 40px;
            color: #1d4999;
        }
    }
    @media (max-width: 768px){
        .col-md-3{
            width: 51%;
            margin: 0 auto;
        }
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
