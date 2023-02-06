<script setup></script>
<template>
    <div class="custom-card">
        <img src="../assets/img1.jpeg" alt="" class="img">
        <div class="content">
            <h2>keep Smiling</h2>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.
                At enim?</p>
        </div>
    </div>

</template>
<style scoped>
.custom-card {
    width: 300px;
    height: 200px;
    border-radius: 10px;
    position: relative;
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.5);
    padding: 30px 50px;
    transition: 0.3s;
    background-color: #fff;
}

.img {
    position: relative;
    width: 100%;
    height: 100%;
    transform: translateY(-70px);
}

img {
    width: 100%;
    border-radius: 10px;
}

.content {
    display: flex;
    transform: translateY(-60px);
    flex-direction: column;
    text-align: center;
}

.content h2 {
    text-transform: uppercase;
    width: 100%;
    font-size: 1.6em;
    color: #333;
}

.content p {
    text-transform: capitalize;
    width: 100%;
    font-size: 0.5em;
    color: #333;
    letter-spacing: 1px;
}

.custom-card:hover {
    background-color: #ff014f;
    transition: all ease-in-out .5s;
    cursor: pointer;
    color: #fff;
}
</style>