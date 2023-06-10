<script setup>

const props = defineProps({
    "url": String,
    "name": String,
    "description": String
});

</script>
<template>
    <a :href="url" target="_blank" class=" block h-full">
        <div class="bg-white rounded-lg shadow-md p-4 w-full sm:w-1/2 md:w-1/4 lg:w-96 hover:shadow-sm hover:bg-gray-50 h-full">
            <h3 class="text-xl font-semibold">{{ name }}</h3>
            <span class=" italic text-gray-500 group-hover:underline">{{ url }}</span><br>
            <span>{{ description }}</span>    
        </div>
    </a>
</template>