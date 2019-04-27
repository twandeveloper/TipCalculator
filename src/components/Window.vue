<template>
    <div id="window">
    <app-bill :bill="bill"></app-bill>
    <app-party :party="party"></app-party>
    </div>
</template>

<script>
import Bill from './Bill.vue'
import Party from './Party.vue'

export default {
    data(){
        return{
            bill: 0,
            party: 0
        }
    },
    components:{
        appBill: Bill,
        appParty: Party
    }

}
</script>
<style scoped>
    #window{
        border: 1px solid #000;
    }
</style>


