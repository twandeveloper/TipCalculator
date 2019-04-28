<template>
<div>
    <div v-if="serviceSubmit">
        <label for="">How good was the service?</label>
        <input type="text" class="form-control-lg" v-on:keyup.enter="submit" v-model="service">
    </div>
    <div v-else>
        <p>{{ service }}</p>
    </div>
</div>
</template>

<script>
export default {
    props:['service'],
    data(){
        return{
            serviceSubmit: true
        }
    },
    methods:{
        submit(){
            this.serviceSubmit = false;
        }
    }
}
</script>

