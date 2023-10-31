<template>
    <article class="tweet border-b border-gray-600">
        <router-link to="#" class="flex p-4">
            <figure class="w-16 mr-3">
                <img :src="tweet.author.profile_img_url" alt="Image" class="rounded-full w-full" />
            </figure>
        </router-link>
    </article>
</template>

<script>
    export default {
        name: 'TheTweet',
        props: ['tweet']
    }
</script>