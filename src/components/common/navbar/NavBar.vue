<template>
	<div class="nav-bar">
    <div class="left"><slot name="left"></slot></div>
    <div class="center"><slot name="center"></slot></div>
    <div class="right"><slot name="right"></slot></div>
  </div>
</template>

<script>
    export default {
        name: "NavBar",
        components: {},
        props: {},
        data() {
            return {}
        },
        computed: {},
        watch: {},
        created() {
        },
        mounted() {
        },
        methods: {}
    }
</script>

<style scoped>
  .nav-bar {
    position: relative;
    z-index: 10;
    display: flex;
    height: 44px;
    line-height: 44px;
    text-align: center;

    border-bottom: 1px solid #eee;
    box-shadow: 0 1px 1px rgba(100,100,100,.08);
  }

  .left {
    width: 60px;
  }

  .center {
    flex: 1;
  }

  .right {
    width: 60px;
  }
</style>
