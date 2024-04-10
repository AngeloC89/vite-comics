<template>
    <header>
        <div id="nav">
            <h1>ciolla</h1>
            <ul>
                <li><a href="#">link</a></li>
                <li><a href="#">link</a></li>
                <li><a href="#">link</a></li>
            </ul>
        </div>
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',

    }
</script>

<style lang="scss" scoped>

    header {
        border: 1px solid red;
        height: 100px;
        width: 100%;
        margin: o auto;
        display: flex;
        align-items: center;

        #nav{
            border: 1px solid red;
            width: 80%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;

            ul{
                display: flex;

                li{
                    list-style: none;
                    text-decoration: none;
                    
                    margin: 20px;
                }
            }
        }
    }
</style>
