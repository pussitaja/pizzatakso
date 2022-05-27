<template>
    <div class="banner" :class="[pos === 'bottom' ? 'bottom' : pos === 'right' ? 'right' : pos === 'left' ? 'left' : 'center']">
        <a href="mailto:reklaamipizzataksos@gmail.com">
            <img v-if="img" :src="img" :width="w" :height="h" />
        </a>
    </div>
</template>

<script>
    export default {
        props: ['w', 'h', 'img', 'pos']
    }
</script>

<style lang="scss">
    .banner {
        position: fixed;
        width: v-bind(w);
        height: v-bind(h);
        border: 2px solid RED;
        z-index: 100;
        &.left {
            left: 10px;
            top: 50%;
            transform: translateY(-50%);
        }
        &.right {
            right: 10px;
            top: 50%;
            transform: translateY(-50%);
        }
        &.bottom {
            left: 50%;
            transform: translateX(-50%);
            bottom: 0px;
        }
    }
</style>