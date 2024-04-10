<template>
    <div class="footertop p-5">
        <div class="container">
            <ul class="d-flex justify-content-around align-items-center list-unstyled">
                <li v-for="(item, index) in MenuFooter" :key="index">
                    <img :src="item.icon" alt="Image" />
                    <a class="text-decoration-none mx-3 text-uppercase" href="#">{{
                        item.text
                        }}</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "FooterTop",
        data() {
            return {
                MenuFooter: [
                    {
                        icon: "/img/buy-comics-digital-comics.png",
                        text: "digital comics",
                        url: "",
                    },
                    {
                        icon: "/img/buy-comics-merchandise.png",
                        text: "dc merchandise",
                        url: "",
                    },
                    {
                        icon: "/img/buy-comics-subscriptions.png",
                        text: "subscription",
                        url: "",
                    },
                    {
                        icon: "/img/buy-comics-shop-locator.png",
                        text: "comic shop locator",
                        url: "",
                    },
                    {
                        icon: "/img/buy-dc-power-visa.svg",
                        text: "dc power visa",
                        url: "",
                    },
                ],
            };
        },
    };
</script>

<style lang="scss" scoped>
    @use '/src/assets/styles/partials/variables' as *;

    body {}

    .footertop {
        background-color: $backgroundFooterTop;

        ul {
            a{
                color: white;

                &:hover {
                   color: rgb(208, 208, 208);
                }
            }
        }
    }

    img {
        height: 50px;
    }
</style>
