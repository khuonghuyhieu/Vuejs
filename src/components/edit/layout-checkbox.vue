<template>
    <div class="row">
        <EditColor />
        <EditAutomation />
    </div>
</template>


<script>
import EditColor from './edit-color.vue';
import EditAutomation from './edit-automation.vue';

export default {
    components:{
        EditColor, EditAutomation
    }
}
</script>