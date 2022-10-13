<template>
    <video class="video" controls>
        <source src="/pizzatakso.mp4" type="video/mp4" />
    </video>
</template>

<style lang="scss">
    .video {
        width: 90%;
        max-width: 500px;
        height: auto;
        border: none;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        z-index: 10;
        border: 3px solid RED;
    }
</style>