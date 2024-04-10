<template>
    <div>
        <div id="list"></div>
        <div id="dc-comics"></div>
    </div>
</template>

<script>
    export default {
        name: 'FooterMid',
        data() {
            return {
                
            }
        },
        
    }
</script>

<style lang="scss" scoped>

div{height: 500px;
    background-image: url('/img/footer-bg.jpg');
    border: 1px solid red;
    display: flex;
    #list{
        width: 50%;
    }
    #dc-comics{
        width: 50%;
        background-image: url('/img/dc-logo-bg.png');
        background-position: center;
        background-repeat: no-repeat;
        background-size: 70%;
     
    }
}

</style>