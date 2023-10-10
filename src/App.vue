
<template>
    <div class="w-[50%] h-[50vh] bg-white flex items-center justify-center rounded-lg">
        <h1 class=" max-sm:text-2xl max-md:text-4xl text-6xl text-center" v-if="name == null">You did not enter your name
        </h1>
        <h1 class=" max-sm:text-2xl max-md:text-4xl text-6xl text-center" v-else-if="name.length > 0">Hello : {{ name }}!
        </h1>
        <h1 class=" max-sm:text-2xl max-md:text-4xl text-6xl text-center" v-else>You did not enter your name</h1>
    </div>
</template>

<script>
export default {
    data() {
        return {
            name: prompt("Please enter your name:"),
        }
    },
}
</script>

<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
</style>
