<template>
    <div class="logo">
        <img src="/logo.gif" alt="logo" />
    </div>
</template>

<style lang="scss">
    .logo {
        width: 300px;
        animation: pizzaRotate 10s infinite linear;
        position: absolute;
        top: 20px;
        z-index: 100;
        pointer-events: none;
        img {
            width: 100%;
        }
    }
</style>