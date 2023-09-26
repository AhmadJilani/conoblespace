<template>
    <NuxtLink :to="to" class="button button-full text-center text-end">
        <div class="container">
            <slot></slot>
            <i class="fa-solid fa-caret-right" style="top: 4px"></i>
        </div>
    </NuxtLink>
</template>
<script>
export default {
    props: {
        to: {
            type: String,
            default: "/forms/membership",
        },
    },
};
</script>
