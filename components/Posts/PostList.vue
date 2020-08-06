<template>
    <section class="posts-list">
        <PostPreview 
            id="1"
            :is-admin="isAdmin"
            thumbnail="https://tech-boys.com/wp-content/uploads/2019/12/womenintech.jpg"
            title="First"
            previewText="This is my first post!" />
        <PostPreview 
            id="2"
            thumbnail="https://tech-boys.com/wp-content/uploads/2019/12/womenintech.jpg"
            title="Second"
            previewText="This is my second post!" />
        <PostPreview 
            id="3"
            thumbnail="https://tech-boys.com/wp-content/uploads/2019/12/womenintech.jpg"
            title="Third"
            previewText="This is my third post!" />
    </section>
</template>

<script>
import PostPreview from '~/components/Posts/PostPreview'

export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style scoped>
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>