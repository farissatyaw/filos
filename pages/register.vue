<template>
    <div class="h-screen p-4 bg-red flex flex-col">
        <div class="mt-3">
            <div class="">
                <h1 class="text-4xl font-bold ml-4">Daftar</h1>
            </div>
            <div class="">
                <div class="card p-4 my-6 flex flex-col">
                    <p>Nama : </p>
                    <input class="input-line" type="text" name="name" >
                    <p>Email : </p>
                    <input class="input-line" type="text" name="email" >
                    <p>Username : </p>
                    <input class="input-line" type="text" name="username" >
                    <p>Password : </p>
                    <input class="input-line" type="text" name="password" >
                    <p>Jenis Kelamin : </p>
                    <input class="input-line" type="text" name="password" >
                    <label class="inline-flex items-center mb-3">
                        <input type="checkbox" class="form-checkbox h-5 w-5 text-gray-600" checked><span class="ml-2 text-xs text-gray-700">Saya Setuju Dengan S&K Berlaku</span>
                    </label>
                    <button class="bg-blue px-4 py-1 rounded-lg mt-3"><span class="text-white">Login</span></button>
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
    }
}
</script>
<style>
.half{
    height: 50vh;
}
.input-line{  
    border-bottom: 1px solid #858586;
    @apply mb-5
}
.bg-red{
    background-image: url(~/assets/img/image14.png);
    background-size: cover;
}
.bg-blue{
    background-color: #0D1B46;
}
.card{
    background-color: rgba(255,255,255, 0.7);
    @apply rounded-lg shadow-2xl;
}
input{
    background: none;
}
</style>