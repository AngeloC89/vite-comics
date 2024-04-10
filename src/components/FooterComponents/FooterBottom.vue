<template>
    <div id="footerbottom">
        <div class="container d-flex justify-content-between align-items-center">
            <button class="text-uppercase">sign up now!</button>
            <div class="d-flex align-items-center">
                <div id="follow" class="text-uppercase fs-4 fw-bold  ">follow us</div>
                <a href=""> <img class="img-fluid" src="/img/footer-facebook.png" alt="Image"></a>
                <a href=""> <img class="img-fluid" src="/img/footer-twitter.png" alt="Image"></a>
                <a href=""> <img class="img-fluid" src="/img/footer-youtube.png" alt="Image"></a>
                <a href=""> <img class="img-fluid" src="/img/footer-pinterest.png" alt="Image"></a>
                <a href=""> <img class="img-fluid" src="/img/footer-periscope.png" alt="Image"></a>


            </div>

        </div>

    </div>
</template>

<script>
    export default {
        name: 'FooterBottom',
        data() {
            return {
            }
        },
    }
</script>

<style lang="scss" scoped>
    @use '/src/assets/styles/partials/variables' as *;

    #footerbottom {
        background-color: $backgroundFooterBottom;

        button {
            padding: 10px;
            border: 2px solid $backgroundFooterTop;
            background-color: $backgroundFooterBottom;
            color: white;
            margin: 30px 0px;

            &:hover {
                background-color: $backgroundFooterTop;
            }
        }

        div {
            #follow {
                color: $backgroundFooterTop;
                margin-right: 10px;
            }

            img {
                margin: 0px 10px;
            }
        }
    }

</style>