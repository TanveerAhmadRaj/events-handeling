<script setup>
</script>
<template>
    <nav class="navbar navbar-expand-lg navbar-dark custom-bg p-3">
        <RouterLink class="navbar-brand" to="/">Septem Systems</RouterLink>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item active">
                    <RouterLink class="nav-link" :to="{ name: 'home' }">Events <span class="sr-only">(current)</span>
                    </RouterLink>
                </li>
                <li class="nav-item">
                    <RouterLink class="nav-link" :to="{ name: 'login' }">Login</RouterLink>
                </li>
                <li class="nav-item">
                    <RouterLink class="nav-link" :to="{ name: 'register' }">Register</RouterLink>
                </li>
                <li class="nav-item">
                    <RouterLink class="nav-link" :to="{ name: 'create' }">Create New</RouterLink>
                </li>
                <li class="nav-item">
                    <button class="nav-link btn">Logout</button>
                </li>
            </ul>

        </div>
    </nav>
</template>
<style scoped>
.custom-bg {
    width: 100%;
    background-image: linear-gradient(to right, #8b33c5, #14a0e1);
}
</style>