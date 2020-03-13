<template>
    <div id="body">
        <button id="buttonOne">This is the first button</button>
        <button id="buttonOne">This is the second button</button>
        <button id="buttonOne">This is the third button</button>
    </div>
</template>

<script>
export default {
    name: 'myBody',
    props: {
        msg: String
    }
}
</script>

<style scoped>
#body{ 
    height: 80vh;
    width:100%;
    border-bottom: solid 1px grey;
}
</style>