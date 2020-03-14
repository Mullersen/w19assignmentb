<template>
    <div id="footer">
        <p>{{msg}}</p>
    </div>
</template>

<script>
export default {
    name: 'myFooter',
    props: {
        msg: String
    }
}
</script>

<style scoped>
#footer{ 
    height: 10vh;
    width:100%;
    background-color: grey;
    border-top: solid 1px grey;
}
</style>