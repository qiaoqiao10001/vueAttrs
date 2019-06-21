<template>
<div class="child-2">
    <p>in child2:</p>
    <p>props: {{pChild2}}</p>
    
    <hr>
</div>
</template>

<script>
export default {
    props: ['pChild2'],
    data() {
        return {};
    },
    inheritAttrs: false,
    mounted() {
        this.$emit('test2','child2 传递到App');
    }
};
</script>
