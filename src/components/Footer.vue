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
#header{ 
    height: 10vh;
    width:100%;
    background-color: grey;
}
</style>