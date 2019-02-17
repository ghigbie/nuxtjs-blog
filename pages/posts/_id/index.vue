<template>
    <div class="single-post-page">
        <section class="post">
            <h1 class="post-title">{{ this.title }} with ID: {{ $route.params.id }}</h1>
            <div class="post-details">
                <div class="last-updated">{{ this.date }}</div>
                <div class="author">{{ this.author }}</div>
            </div>
            <p class="content">{{ this.postContent }}</p>
        </section>
        <section class="post-feedback">
            {{ this.feedback }}
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

</style>
