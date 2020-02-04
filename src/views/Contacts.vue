<template>
    <footer class="contacts">
        <a name="contacts"></a>
        <div class="container">
            <div class="contacts__row">
                <div class="contacts__infoblock">
<pre class="contacts__title">
For questions
and suggestions
</pre>
                    <Contact class="contacts__contact-style1" ico="envelope.png" info="email@shelter.com"/>
                    <Contact ico="telephone.png" info="+13 674 567 75 54"/>
                </div>
                <div class="contacts__infoblock">
<pre class="contacts__title">
We are waiting
for your visit
</pre>
                    <Contact class="contacts__contact-style1" ico="pin.png" info="Boston, Central Street, 1st (Entrance from the store)"/>
                    <Contact ico="pin.png" info="London, South Park, 18st"/> <!-- /.contacts__title -->
                </div>
                <img class="contacts__image" src="@/assets/images/dog_11544.png" alt="">
            </div>
        </div>
    </footer>
</template>

<script>
    import Contact from "../components/Contact";
    export default {
        name: "Contacts",
        components: {
            Contact
        }
    }
</script>

<style scoped lang="scss">
    .container{
        max-width: 1163px;
        margin: 0 auto;
        padding: 0 10px 0 10px;
    }
    .contacts{
        max-width: 100%;
        background: url(../assets/images/background.jpg) no-repeat;
        background-size: cover;
        &__row{
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }
        &__infoblock{
            width: 292px;
            padding: 79px 0 79px 0;
            display: flex;
            flex-direction: column;
            @media (max-width: 768px) {
                padding: 20px 0 20px 0;
            }
        }
        &__title{
            margin-bottom: 40px;
            font-family: Georgia;
            font-size: 35px;
            line-height: 45px;
            font-weight: 400;
            letter-spacing: 0.06em;
            color: #ffffff;
        }
        &__contact-style1{
            margin-bottom: 34px;
        }
        &__image{
            margin-top: 49px;
        }
    }

</style>
