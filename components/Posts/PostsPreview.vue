<template>
    <nuxt-link :to="'/posts' + 2" class="post-preview">
        <article>
          <div class="post-thumbnail"
               style="background-image: url('https://www.topuniversities.com/sites/default/files/articles/lead-images/mit_vs_caltech.jpg')">
          </div>
          <div class="post-content">
            <h1>Post Title</h1>
            <p>Preview Text</p>
          </div>
        </article>
    </nuxt-link>
</template>
