<script setup></script>
<template>
    <div class="grid">
        <section class="side">
            <img src="../assets/img.svg" alt="">
        </section>
        <section class="main">
            <div class="login-container">
                <p class="title">Sign up</p>
                <div class="seperator"></div>
                <p class="login-message">
                    Please, Sign Up Using Email and Password
                </p>
                <form class="login-form">
                    <div class="forms-control">
                        <input type="text" placeholder="Username">
                        <i class="fa fa-user"></i>
                    </div>
                    <div class="forms-control">
                        <input type="password" placeholder="Password">
                        <i class="fa fa-lock"></i>
                    </div>
                    <button class="submit">register</button>
                </form>
            </div>
        </section>
    </div>
</template>
<style scoped>
.grid {
    min-height: 90vh;
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr;
}

section {
    display: flex;
    justify-content: center;
    align-items: center;
}

section.side {
    background: url(../assets/bk.png) no-repeat;
    background-size: 100% 102%;
}

.side img {
    width: 50%;
    max-width: 50%;
}

.login-container {
    max-width: 450px;
    padding: 24px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.title {
    text-transform: uppercase;
    font-size: 3em;
    text-align: center;
    list-style: 1px;
    font-weight: 600;
}

.seperator {
    width: 150px;
    height: 4px;
    margin: 10px 24px;
    background-color: #843bc7;
}

.login-message {
    text-align: center;
    margin-bottom: 30px;
    font-size: 1.1em;
    color: #696969;
    line-height: 28px;
}

.login-form {
    width: 100%;
    display: flex;
    flex-direction: column;

}

.forms-control {
    width: 100%;
    margin-bottom: 24px;
    position: relative;
}

input,
button {
    border: none;
    outline: none;
    font-size: 1.1em;
    border-radius: 30px;
}

input {
    width: 100%;
    background-color: #e6e6e6;
    color: #333;
    padding: 14px 65px;
}

input~i {
    position: absolute;
    top: 50%;
    left: 32px;
    transform: translateY(-50%);
    color: #888;
    transition: color 0.4s;
}

input:focus~i {
    color: #843bc7;
}

button.submit {
    color: #fff;
    padding: 14px 64px;
    list-style: 2px;
    text-transform: uppercase;
    font-weight: bold;
    margin: 32px auto;
    background-image: linear-gradient(to right, #8b33c5, #14a0e1);
    cursor: pointer;
    transition: opacity 0.4s;
    ;
}

button.submit:hover {
    opacity: 0.9;
}

@media (max-width: 780px) {
    .grid {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .side {
        display: none;
    }
}
</style>