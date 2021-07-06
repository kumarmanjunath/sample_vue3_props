<template>
    <div class="home">
        <h1>Home Sweet Home</h1>
        <PostList :posts="posts"/>
    </div>
</template>

<script>
import {ref} from 'vue'
import PostList from './PostList.vue'
export default {
    name:'Home',
    components:{PostList},
    setup () {
        const posts=ref([
      {title:'welcome to the blog', body:'Loremd fff',id:1},
       {title:'top 5 css tips', body:'Loremd ddd',id:2}
    ])
        

        return {posts}
    }
}
</script>

<style lang="scss" scoped>

</style>