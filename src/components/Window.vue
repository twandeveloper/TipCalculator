<template>
    <div id="window" class="form-group">
        <app-bill :bill="bill"></app-bill>
        <app-party :party="bill"></app-party>
        <app-service :service="service"></app-service>
    </div>
</template>

<script>
import Bill from './Bill.vue'
import Party from './Party.vue'
import Service from './Service'

export default {
    data(){
        return{
            bill: 0,
            party: 2,
            service: 0
        }
    },
    components:{
        appBill: Bill,
        appParty: Party,
        appService: Service
    }

}
</script>
<style scoped>
    #window{
        /* border: 1px solid #000; */
        box-shadow: 5px 10px 8px 10px #888888;
        width: 400px;
        margin: 10px auto;
    }
 
</style>


