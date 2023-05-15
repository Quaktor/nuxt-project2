<template>
  <div>
    <div style="background-color: #b7e2ff;">
    <TopNav/>
    
    <BigImg image="https://cdn.pixabay.com/photo/2019/08/19/07/45/corgi-4415649_960_720.jpg" />
    <BigImg image="https://cdn.pixabay.com/photo/2020/03/31/19/20/dog-4988985_960_720.jpg" />
    </div>
  </div>
</template>

<script>
import BigImg from '~/components/gallery/BigImg.vue';
import TopNav from '~/components/navi/TopNav.vue';

export default {
    name: "IndexPage",
    components: { TopNav, BigImg }
}
</script>

<style scoped>
</style>
