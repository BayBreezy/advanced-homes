<template>
	<div>
		<NuxtPage />
	</div>
</template>

<script setup>
	useHead({
		title: "Advanced Homes",
		meta: [
			{
				name: "description",
				content: "Advanced Homes - Let us help you make the transition",
			},
			{
				property: "og:title",
				content: "Advanced Homes",
			},
			{
				property: "og:description",
				content: "Advanced Homes - Let us help you make the transition",
			},
			{
				property: "og:image",
				content: "/home.jpg",
			},
			{
				property: "og:type",
				content: "website",
			},
			{
				property: "og:site_name",
				content: "Advanced Homes",
			},
		],
	});
</script>
