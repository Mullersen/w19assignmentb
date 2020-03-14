<template>
<div>
    <p v-on:click="makeRed">{{ author }}</p>
    <p> {{ content}} </p> <!-- vue is calling the data function/method for us. we never call it ourselves. -->
</div>
</template>

<script>
export default {
    name: 'Tweet',
    props: {
        author: { // is a JS-object ( key-value pair) that contains a set of properties that can make the "author" field dynamic.
            type: String, 
            required: false, 
            default: 'Author'
        }
    },
    methods: {
        makeRed : function(){
            document.body.style.backgroundColor = "red"
        }
    }, 
    data: function(){
        return {
            content: "this is the tweet content"
        }
    }
}
</script>

<style scoped>

</style>