<template>
     <div>
        <div v-if="billSubmit">
            <label for="">How much was the Bill?</label>
            <input type="text" class="form-control-lg " v-on:keyup.enter="submit" v-model="bill" >
        </div>
        <div v-else>
            <h2>${{ bill }}</h2> 
        </div>
    </div>
</template>

<script>
export default {
    props:['bill'],
    data(){
        return{
            billSubmit: true
        }
    },
    methods:{
        submit(){
            this.billSubmit = false;
        }
    },
    computed: {

    }
}
</script>

