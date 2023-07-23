<template>
<Link href="/listing">Listing</Link>&nbsp;
<Link href="/listing/create">New Listing</Link>

<!-- <div>{{ timer }}</div> -->
<div v-if="flashSuccess" class="success">
{{ flashSuccess }}
</div>
<slot>Default</slot>

</template>

<script setup>
import {Link, usePage} from '@inertiajs/vue3'
import { ref } from 'vue';
import { computed } from 'vue';
const flashSuccess = computed(
    ()=>page.props.flash.success
)
const page = usePage()



</script>

<style scoped>
.success{
    background-color: rgb(79, 227, 53);
    color: white;
}
</style>