<template>
    <div class="h-screen">
        <div class="navbar">
            <img class="logo" src="../assets/ayam_logo.svg" alt="logo"/>
        </div>

        <div class="grid flex justify-center md:grid-cols-12">
            <div class="md:col-span-6 lg:col-span-7 flex justify-center">
                <div class="container flex justify-center p-20">
                    <img class="h-64 md:h-auto object-contain" src="../assets/img/login_vector.png" alt="login"/>
                </div>
            </div>
            <div class="md:col-span-6 lg:col-span-5 md:h-screen flex md:items-center">
                <div class="container md:pt-0 md:pb-20">
                    <h1>Welcome</h1>
                    <h2 class="font-light">Sign in to BINUSMaya</h2>
                    <login-form/>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import LoginForm from "../components/LoginForm";
    export default {
        name: "Login",
        components: {LoginForm}
    }
</script>

<style scoped>
    .navbar {
        @apply relative h-16 py-1 px-6 text-gray-900 text-left float-none fixed flex justify-between items-center z-30;
        width: 100vw;
    }
    .logo {
        @apply h-full pt-3 pb-3 object-scale-down object-left;
    }
</style>
