<template>
    <article class="tweet border-b border-gray-600">
        <router-link to="#" class="flex p-4">
            <figure class="w-16 mr-3">
                <img :src="tweet.author.profile_img_url" alt="Image" class="rounded-full w-full" />
            </figure>
            <section class="tweet-body flex-1">
                <div class="tweet-author">
                    <span class="text-white font-bold">{{ tweet.author.display_name }}</span>
                    <span class="text-gray-500 ml-2 font-normal">{{ tweet.author.username }}</span>
                </div>
            </section>
        </router-link>
    </article>
</template>

<script>
    export default {
        name: 'TheTweet',
        props: ['tweet']
    }
</script>