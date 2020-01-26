<template>
    <div class="button"
         v-bind:class="{ button_ispressed: isPressed,
                         button_ismove: isMove,
                         button_isbig: big,
                         button_issmall: small }"
         @mousedown="isPressed=true"
         @mouseup="isPressed=false"
         @mousemove="isMove=true"
         @mouseleave="isMove=false">
        <span class="button__label"
              v-bind:class="{ button__label_isblack: black }">
            {{ label }}
        </span>
    </div>
</template>

<script>
    export default {
        name: "button",
        props: {
            'label': String,
            'black': Boolean,
            'big': Boolean,
            'small': Boolean
        },
        data () {
            return {
                isPressed: false,
                isMove: false
            }
        },
    }
</script>

<style scoped lang="scss">
    .button {
        width: 205px;
        height: 52px;
        border: 1px solid #f1cdb3;
        border-radius: 26.0px;
        text-align: center;
        cursor: pointer;
        &__label {
            font-family: Georgia;
            font-size: 17px;
            line-height: 52px;
            font-weight: 400;
            letter-spacing: 0.06em;
            color: white;
            &_isblack{
                color: #292929;
            }
        }
        &_ispressed{
            background-color: #f1cdb3;
            & :first-child{
                color: #292929;
            }
        }
        &_ismove{
            border: 2px solid #f1cdb3;
        }
        &_isbig{
            width: 267px;
        }
        &_issmall{
            width: 50px;
            & :first-child {
                font-family: 'Material Icons';
                font-size: 38px;
                line-height: 52px;
                letter-spacing: normal;
            }
        }
    }
</style>
