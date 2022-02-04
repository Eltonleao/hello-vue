<template>
<h2>Options - {{ o_firstName }}</h2>
<h2>Composition - {{ c_firstName }}</h2>

  
</template>

<script>

import { ref, reactive } from "vue";

export default {
    name: "Data",
    reactive:{
        o_firstName: ref("John"),
        c_firstName: ref("Doe")
    },
    }

    setup(){
        const c_firstName =  ref('Clark');



        return {
            c_firstName
        }
    },
    data(){
        return{
            o_firstName: "John",
        }
    }

}
</script>

<style>

</style>