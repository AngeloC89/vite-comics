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

div{
    border: 1px solid red;
    display: flex;
    #list{height: 100px;
        width: 50%;
    }
    #dc-comics{height: 100px;
        width: 50%;
    }
}

</style>