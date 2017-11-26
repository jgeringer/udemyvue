<template>
    <div>
        <p>Server Status {{status}}</p>
        <hr>
        <button @click="changeStatus">Change Status</button>
    </div>
</template>

<script>
    //Local component
    export default{
        data: function(){
            return{
                status: 'Critical'
            }
        },
        methods: {
            changeStatus(){ //es6
                this.status = 'Normal' 
            }
        }
    }
</script>

<style scoped>
    div {
        border: 1px solid blue;
    }
</style>