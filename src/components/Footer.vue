<script setup>
const profiles = [
	{
		url: 'https://github.com/octocat',
		icon: `<svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>Facebook</title><path d="https://www.facebook.com/lin.homebs"/></svg>`
	}
]
</script>
<template>
	<div class="flex flex-row items-center justify-center my-8 w-full">
		<a :href="profile.url" class="w-6 h-6"
		   v-for="(profile, i) in profiles" :key="i" v-html="profile.icon"></a>
	</div>
</template>
