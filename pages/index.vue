<template>
  <div>
    <h3 class="page-title">Current page List</h3>
    <div class="recent-posts" v-if="page.posts">
      <ul>
        <li v-for="post in page.posts" :key="post.permalink">
          <h2>
            <a :href="post.permalink">{{
              post.title
            }}</a>
          </h2>

          <p class="card-text" v-if="post.college">
              <strong>Studies in: </strong>{{post.college}}
          </p>

          <p class="card-text" v-if="post.interests">
            <strong>Interested in: </strong>
            <span v-for="interest in post.interests" :key="interest">{{interest}}, </span>
          </p>

        </li>
      </ul>
    </div>
  </div>
</template>

<script>
    export const data = {
    layout: 'page',
    injectAllPosts: true
    }

    export default {
        props: ['page'],
        methods: {
            formatDate(v) {
                const date = new Date(v)
                return `${date.getFullYear()}/${date.getMonth() + 1}/${date.getDate()}`
            }
        }
    }
</script>


<style scoped>
    .page-title{
        font-weight: normal;
        font-size: 1.5rem;
        margin-bottom: 10px;
    }
    ul{
        list-style: none;
    }

    li{
        border: 2px solid #ccc;
        padding: 20px;
    }

    a{
        text-decoration: none;
        color:#2e0085;
    }

    .card-text{
        margin-top: 10px;
    }
</style>