<template>
    <layout>
        <br><br>
        <g-image :src="$page.blogPost.cover_img" style="width:100%" />
        <h1>{{ $page.blogPost.title }} </h1>
        <h4>{{ $page.blogPost.date }}</h4>
        <div v-html=" $page.blogPost.content "></div>
        <v-btn color="secondary">{{ $page.blogPost.category }} </v-btn>
    </layout>
</template>

<page-query>
query ($path: String!) {
    blogPost(path: $path) {
        category
        title
        content
        date
        tags
        cover_img(width: 500, height: 280)
    }
}

</page-query>