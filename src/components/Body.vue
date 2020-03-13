<template>
<div id="body-container">
    <div class="body">
        <button v-on:click="hello" id="buttonOne">This is the first button</button>
    </div>
    <div class="body">
        <button v-on:click="background" id="buttonTwo">This is the second button</button>
    </div>
    <div class="body">
        <button v-on:click="move" id="buttonThree">This is the third button</button>
    </div>
</div>
</template>

<script>

export default {
    name: 'myBody',
    props: {
        msg: String
    },
    methods: {
        hello: function(){
            var newChild = document.createElement('p');
            var content = document.createTextNode('Hello there, you look nice today!');
            newChild.appendChild(content);
            document.getElementById('body-container').appendChild(newChild);
        },
        background: function(){
            document.getElementById('body-container').style.backgroundColor= "green";
        },
        move: function(){
            var marginCounter = 0;
            var Int = setInterval(function() {
                    console.log(marginCounter);
                    document.getElementById('buttonThree').style.marginTop = marginCounter + "px";
                    marginCounter += 0.1;
                    if (marginCounter >= 100) {
                        clearInterval(Int);
                    }
                }, 10);
        }
    }
}
</script>

<style scoped>
#body-container{ 
    height: 80vh;
    width:100%;
    border-bottom: solid 1px grey;
}
.body{
    height: 20vh;
    width: 50%;
}
</style>