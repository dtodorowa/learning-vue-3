
<template class="post-detail">
  <div>
    <h1>This is a post page</h1>
    <p>Display the content of post with id of {{$route.params.id}} here</p>
    <div>
    <button @click="showPostId">Show Post Id</button>
    </div>
    <div>
    <button @click="goHome">Go Home</button>
    </div>
    <div>
    <button @click="goToFirstPost">Go to first Post</button>
    </div>
    <p><RouterLink to="/posts">&lt; Back</RouterLink></p>
  </div>
</template>

<script setup>
  import { useRoute, useRouter } from 'vue-router';

  const route = useRoute();
  const router = useRouter();

  const showPostId = () => {
    alert(`The ID of this post is: ${ route.params.id }`);
  }

  const goHome = () => {
    router.push('/');
  }

  const goToFirstPost = () => {
    router.push({
      name : 'postDetail',
      params: {
        id: 'id1'
      }
    });
    }
</script>