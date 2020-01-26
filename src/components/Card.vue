<template>
    <div class="card">
        <img src="../assets/images/cat_11858.png" class="card__image">
        <div class="card__name">
            Katrine
        </div>
        <Button label="Learn More" black/>
        <!-- /.card__name -->
    </div>
    <!-- /.card -->
</template>

<script>
    import Button from "./Button";
    export default {
        name: "Card",
        components: {
            Button
        }
    }
</script>

<style scoped lang="scss">
    .card{
        width: 270px;
        height: 424px;
        background-color: #fafafa;
        border-radius: 9.0px;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
        &__image{
            width: 226px;
            height: 226px;
        }
        &__name{
            font-family: Georgia;
            font-size: 20px;
            line-height: 45px;
            font-weight: 400;
            letter-spacing: 0.06em;
            color: #545454;
        }
    }

</style>
