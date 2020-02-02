<template>
<div class="contact">
    <img v-bind:src="resolve_img_url(ico)" alt="">
    <div class="contact__info">
        {{ info }}
    </div>
    <!-- /.contact__info -->
    <!-- /.ico -->
</div>
<!-- /.contact -->
</template>

<script>
    export default {
        name: "Contact",
        props: {
            'ico': String,
            'info': String
        },
        methods: {
            resolve_img_url: function (path) {
                let images = require.context('../assets/images/', false, /\.png$|\.jpg$/)
                return images("./" + path)
            }
        }
    }
</script>

<style scoped lang="scss">
    .contact{
        display: flex;
        align-items: center;
        &__info{
            margin-left: 22px;
            font-family: TimesNewPSMT;
            font-size: 20px;
            line-height: 15px;
            font-weight: 400;
            letter-spacing: 0.06em;
            color: #f1cdb3;
        }
    }

</style>
