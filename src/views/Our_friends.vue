<template>
<div class="friends">
    <div class="container">
        <div class="friends__col">
            <div class="friends__title">
                <span>Our friends who</span>
                <span>are looking for a house</span>
            </div>
            <div class="friends__carusel">
                <Button label="navigate_before" black small></Button>
                <Card></Card>
                <Button label="navigate_next   " black small></Button>


            </div>
            <Button label="Get to know the rest" big black/>
            <!-- /.friends__carusel -->
        </div>
        <!-- /.friends__col -->

    </div>
    <!-- /.container -->
</div>
<!-- /.friends -->
</template>

<script>
    import Button from "../components/Button";
    import Card from "../components/Card";
    export default {
        name: "Our_friends",
        components: {
            Button,
            Card
        }
    }
</script>

<style scoped lang="scss">
    .container {
        max-width: 1060px;
        margin: 0 auto;
    }
    .friends{
        max-width: 100%;
        padding: 78px 0 68px 0;
        height: 833px;
        background-color: #f6f6f6;
        &__col{
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
        }
        &__title{
            max-width: 396px;
            text-align: center;
            font-family: Georgia;
            font-size: 35px;
            line-height: 45px;
            font-weight: 400;
            letter-spacing: 0.03em;
            color: #545454;
        }
        &__carusel{
            height: 424px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
    }
    span{
        display: inline-block;
    }
</style>
