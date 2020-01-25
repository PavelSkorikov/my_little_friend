<template>
    <div class="button">
        <span class="button__label">
            {{ label }}
        </span>
        <!-- /.button__label -->
    </div>
    <!-- /.button -->
</template>

<script>
    export default {
        name: "button",
        props: {
            'label': String
        }
    }
</script>

<style scoped lang="scss">
    .button {
        width: 205px;
        height: 52px;
        background-color: #f1cdb3;
        border-radius: 26.0px;
        text-align: center;
        cursor: pointer;
        &__label {
            font-family: Georgia;
            font-size: 17px;
            line-height: 52px;
            font-weight: 400;
            letter-spacing: 0.06em;
            color: #292929;
        }
    }
</style>
