<template>
    <div class="card">
        <img class="card__image" v-bind:src="resolve_img_url(url)"  alt="">
        <div class="card__name">
            {{ name }}
        </div>
        <Button label="Learn More" black/>
        <!-- /.card__name -->
    </div>
    <!-- /.card -->
</template>

<script>
    import Button from "./Buttons";
    export default {
        name: "Card",
        props: {
            'url': String,
            'name': String
        },
        components: {
            Button
        },
        methods: {
            resolve_img_url: function (path) {
                let images = require.context('../assets/images/', false, /\.png$|\.jpg$/)
                return images("./"+path)
            }
        }
    }
</script>

<style scoped lang="scss">
    .card{
        box-shadow: 0px 2px 30px 5px rgba(13,13,13,0.03);
        width: 270px;
        height: 424px;
        background-color: #fafafa;
        border-radius: 9.0px;
        padding: 33px 0 34px 0;
        background-color: #fafafa;
        border-radius: 9.0px;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
        &__image{

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
