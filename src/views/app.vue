<template>
<div id="app">
    <Child1 
    :p-child1="child1"
     :p-child2="child2"
      v-on:test1="onTest1" 
       v-on:test2="onTest2">
    </Child1>
</div>
</template>

<script>
import Child1 from './Child1.vue';
export default {
    data() {
        return {
            child1:'A 组件的数据1',
             child2:'A 组件的数据2'
        };
    },
    components: {
        Child1
    },
    methods: {
        onTest1() {
            console.log('test1 running...');
        },
        onTest2(v) {
            console.log(v);
        }
    }
};
</script>
