<script>
    export {
    };
</script>

<template>
    <div class="work">
        <h1> workComponent works !<button @click="showDetail">+</button></h1>
        <div v-if="showDetail" id="work-detail">
            <p>ceci est un paragraphe</p>
        </div>
    </div>
</template>

<style>
    #work-detail {
        display:none;
    }
</style>
