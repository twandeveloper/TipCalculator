<template>
    <div>
        <div v-if="partySubmit" class="">
            <div>
                <label for="">How many people are in the party </label>
                <input type="text" class="form-control-lg" v-model="party" v-on:keyup.enter="submit">
            </div>
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
