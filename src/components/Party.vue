<template>
    <div id="party">
        <div v-if="partySubmit">
            <label for="">How many people are in the party </label>
            <input type="text" class="form-control" v-on:keyup.enter="submit">
        </div>
        <div v-else>
            <p>{{ party }}</p>
        </div>
    </div>
</template>

<script>
export default {
    props:['party'],
    data(){
        return{
            partySubmit: true
        }
    },
    methods:{
        submit(){
            this.partySubmit = false;
        }
    }
}
</script>
