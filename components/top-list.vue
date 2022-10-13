<template>
    <div class="top-list">
        <slot />
    </div>
</template>

<style lang="scss">
    .top-list {
        position: absolute;
        bottom: 20px;
        left: 20px;
        padding: 20px;
        background: YELLOW;
        border: 3px solid GREEN;
        font-family: 'Verdana';
        color: RED;
        ol {
                padding: 0;
        }
    }
</style>