<template>
  <div>
    <h3 class="page-title">Current List</h3>
    <div class="recent-posts" v-if="posts">
      <ul>
        <li v-for="post in posts" :key="post.permalink">

          <div v-if="post.image"> 
            <img :src="post.image" alt="post.title">
          </div>

          <div>
            <h2>
              <a :href="post.permalink">{{
                post.title
              }}</a>
            </h2>

            <p class="card-text" v-if="post.institution">
                <strong>Studies/Works in: </strong>{{post.institution}}
            </p>

            <p class="card-text" v-if="post.interests">
              <strong>Interested in: </strong>
              <span v-if="post.interests.length === 0">Nothing Specified!</span>
              <span v-for="interest in post.interests" :key="interest">{{interest}}, </span>
            </p>


            <p class="card-text" v-if="post.socials">
              <strong>Socials: </strong>
              <span v-for="(social,index) in post.socials" :key="index">
                <a :href="social.url">{{social.name}}</a>&nbsp;
              </span>
              
            </p>
          </div>

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
        props: {
          page: {
            type: Object,
            required: true,
          }
        },
        computed: {
          posts() {
            if (this.page.posts) {
              return this.page.posts.sort((postA, postB) => {
                return postA.createdAt.getTime() - postB.createdAt.getTime()
              }).reverse()
            }
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
        margin-bottom: 10px;
        display: flex;
        align-items: flex-start;
        flex-direction: column;
    }

    li img{
      width: 100px;
      margin-right: 40px;
    }

    a{
        text-decoration: none;
        color:#2e0085;
    }

    .card-text{
        margin-top: 10px;
    }


    @media (max-width: 450px){
      li{
        flex-direction: column;
      }

      li img{
        margin: 0;
        margin-bottom: 10px;
      }
    }
</style>
