<template>
    <span class="timestamp">{{timestamp}}</span>
</template>

<script>
export default {
    props: {
        timestamp: {
            type: String,
            default: "19h ago"
      
        }
    }
}
</script>