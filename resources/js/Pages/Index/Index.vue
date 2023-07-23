<template>
    <div>
        Index 
    </div>
    <div>The messages is {{ messages }}</div>
    <Link href="/hello">Show Pages</Link>
</template>

<script setup>
import {Link} from '@inertiajs/vue3'
defineProps({
    messages: String
})
</script>

