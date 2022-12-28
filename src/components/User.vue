<template>
    <span class="name">{{user.name}}</span>
    <span class="handle">{{user.handle}}</span>
</template>

<script>
export default {
    props: {
        user: {
            type: Object,
            default: {
                name: "Default name",
                handle: "default handle"
            }
        }
    }
}
</script>