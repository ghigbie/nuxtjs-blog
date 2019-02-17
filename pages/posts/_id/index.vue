<template>
    <div class="single-post-page">
        <section class="post">
            <h1 class="post-title">{{ this.title }} with ID: {{ $route.params.id }}</h1>
            <div class="post-details">
                <div class="last-updated">{{ this.date }}</div>
                <div class="author">{{ this.author }}</div>
            </div>
            <p class="post-content">{{ this.postContent }}</p>
        </section>
        <section class="post-feedback">
            {{ this.feedback }} <a href="mailto:afaf@moo.com">adfaf@moo.com</a>
        </section>
    </div>
</template>

<script>
export default {
    computed: {
        title(){
            return 'Title of Post';
        },
        author(){
            return 'Author of Post';
        },
        date(){
            return 'Date of Last Updated';
        },
        postContent(){
            return 'Content of post';
        },
        feedback(){
            return 'Feedback on post';
        }

    }
}
</script>


<style>
.single-post-page {
  padding: 30px;
  text-align: center;
  box-sizing: border-box;
}

.post {
  width: 100%;
}

@media (min-width: 768px) {
  .post {
    width: 600px;
    margin: auto;
  }
}

.post-title {
  margin: 0;
}

.post-details {
  padding: 10px;
  box-sizing: border-box;
  border-bottom: 3px solid #ccc;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

@media (min-width: 768px) {
  .post-details {
    flex-direction: row;
  }
}

.post-detail {
  color: rgb(88, 88, 88);
  margin: 0 10px;
}

.post-feedback a {
  color: red;
  text-decoration: none;
}

.post-feedback a:hover,
.post-feedback a:active {
  color: salmon;
}
</style>
