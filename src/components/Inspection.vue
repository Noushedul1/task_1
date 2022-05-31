<template>
    <div class="inspection">
        <h4>
            Title
        </h4>
        <div class="inspectionContent">
            <div class="inspectionCircle one">
                <div class="insideCircle">
                    <h5>
                        1 BN+
                    </h5>
                    <P>
                        Daily Impressions
                    </P>
                </div>
            </div>
            <div class="inspectionCircle two">
                <div class="insideCircle">
                    <h5>
                        &dollar;500K+
                    </h5>
                    <P>
                        Paid
                    </P>
                </div>
            </div>
            <div class="inspectionCircle three">
                <div class="insideCircle">
                    <h5>
                       8K+
                    </h5>
                    <P>
                        Global Publishers
                    </P>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default{
    name: 'Inspection',
    data() {
    
    }
}
</script>
<style lang="scss" scoped>
.inspection{
    min-height: 400px;
    background: #644F9C;
    padding: 30px;
    margin-top: 100px;
    h4{
        text-align: center;
        color: #F2F2F2;
        padding: 15px;
    }
    .inspectionContent{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        .one{
           border: 1px dotted #F2F2F2;
           color: #F2F2F2
        }
        .two{
            background: #F2F2F2;
        }
        .three{
            background: #FF6F00;
            color: #F2F2F2;
        }
        .inspectionCircle{
        height: 200px;
        width: 200px;
        border-radius: 50%;
        margin-top: 40px;
        display: flex;
        justify-content: center;
        align-items: center;
        h5{
            font-size: 35px;
            text-align: center;
        }
        p{
            font-size: 20px;
            text-align: center;
        }
        }
    }
}
</style>