<template>
    <div id="header">
        <p>{{msg}}</p>
    </div>
</template>

<script>
export default {
    name: 'myHeader',
    props: {
        msg: String
    }
}
</script>

<style scoped>
#header{ 
    top:0;
    height: 10vh;
    width:100%;
    background-color: aquamarine;
    border-bottom: solid 1px grey;
}
</style>