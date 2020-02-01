<template>
    <div class="infobanner">
        <img v-bind:src="resolve_img_url(url)" alt="">
        <div class="infobanner__info">
            {{ info }}
        </div>
    </div>
</template>

<script>
    export default {
        name: "Infobanner",
        props: {
            'info': String,
            'url': String
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
    .infobanner {
        text-align: center;
        &__info {
            font-family: Georgia;
            font-size: 20px;
            line-height: 65px;
            font-weight: 400;
            letter-spacing: 0.06em;
            color: #545454;
        }
    }
</style>
