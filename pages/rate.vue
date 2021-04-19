<template>
    <div class="h-screen p-4 bg-turqoise flex flex-col justify-center">
        <div class="mt-3">
            
            <div class="">
                <div class="card p-4 my-6 flex flex-col items-center">
                    <h1 class="text-2xl font-bold">Thank You</h1>
                    <svg class="flex" height="150" width="150">
                        <circle cx="75" cy="75" r="60" stroke="black" stroke-width="0" fill="gray" />
                    </svg>
                    <div class="flex">
                        <button type="button" v-for="i in 5" class="focus:outline-none" :class="{ 'mr-1': i < 5 }" @click="$emit('input', i)">
                        <svg class="block h-8 w-8" :class="[ value >= i ? 'text-blue': 'text-grey']" fill="currentColor" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/></svg>
                        </button>
                    </div>
                </div>
                <div class="flex justify-center">
                    <button class=" bg-button px-10 py-2 font-light text-white rounded-full">Submit</button>
                </div>
            </div>
        </div>  
    </div>
</template>
<script>
export default {
    head(){
        return {
            title: "About the app"
        }
    },
    data: (i) => ({
        rating:3,
    })
}
</script>
<style>
.half{
    height: 50vh;
}
.input-line{  
    border-bottom: 1px solid #858586;
    @apply mb-3
}
.bg-turqoise{
    background-image: url(~/assets/img/image14.png);
    background-size: cover;
}
.bg-blue{
    background-color: #0D1B46;
}
.bg-button{
    background-color: #0E1B47;
}
.card{
    background-color: rgba(255,255,255,0.7);
    @apply rounded-lg shadow-2xl;
}
</style>