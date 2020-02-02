<template>
    <div class="navbaritem" v-on:mouseover="mouseover" v-on:mouseleave="mouseleave">
        <a :href="url" class="navbaritem__label">
            {{ label }}
        </a>
        <div class="navbaritem__underline" v-show="isHover">
        </div>
        <!-- /.navbaritem__underline -->
        <!-- /.navbaritem__label -->
    </div>
    <!-- /.navbaritem -->
</template>

<script>
    export default {
        name: "NavbarItem",
        props: {
            'label': String,
            'url': String
        },
        data () {
            return {
                isHover: false
            }
        },
        methods: {
            mouseover: function(){
                this.isHover = true
            },
            mouseleave: function(){
                this.isHover = false
            }
        }
    }

</script>

<style scoped lang="scss">
    .navbaritem {
        height: 32px;
        display: flex;
        flex-direction: column;
        cursor: pointer;
        &__label {
            font-family: ArialMT;
            font-size: 15px;
            line-height: 29px;
            font-weight: 400;
            white-space: nowrap;
            color: #cdcdcd;
        }
        &__underline {
            height: 3px;
            background-color: #f1cdb3;
            border-radius: 1.5px;
        }
    }

</style>
