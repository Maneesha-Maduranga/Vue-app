<script>
export default {
    methods:{
        toggle(){
            this.$refs.btn.classList.add('none')
        }
    }
}
</script>


<template>
    <div class="modal" ref="btn">
        <button class="close" @click="toggle" >Close</button>
        <h1>Modal Header</h1>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Amet officia quisquam molestias et ullam odit totam error, modi consectetur saepe?</p>
    </div>
</template>

<style>
    .modal{
        height: 150px;
        width: 30%;
        background-color:aliceblue;
        color: black;
        border-radius: 10px;
        text-align: center;
        padding: auto;
        position: relative;
        margin: auto;
    }
    .close{
        position: absolute;
        right: 25px;
        top: 10px;
        background-color: tomato;
        color: #fff;
        border-radius: 5px;
    }
    .close:hover{
        background-color: #fff;
    }
    .none{
        visibility: hidden;
    }
   
</style>
