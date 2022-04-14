<template>
	<header
		class="flex items-center justify-between h-20 lg:max-w-6xl mx-auto px-5 lg:px-0"
	>
		<!-- Logo -->
		<NuxtLink to="/">
			<IconLogo class="w-14 h-14" />
		</NuxtLink>
		<!-- Nav -->
		<ul class="md:flex items-center space-x-3 hidden">
			<template :key="`Navitem${i}`" v-for="(n, i) in nav">
				<li>
					<NuxtLink
						class="inline-block px-3 py-2 hover:bg-slate-200 transition-all duration-300 bg-gray-50 rounded-full text-sm"
						to="#"
						>{{ n.text }}</NuxtLink
					>
				</li>
			</template>
		</ul>
		<NuxtLink
			to="#"
			class="px-5 py-2 text-sm bg-violet-700 text-white rounded-full hover:bg-violet-900 transition-all duration-300"
			>Download App</NuxtLink
		>
	</header>
</template>
<script setup>
	const nav = [
		{
			text: "Home",
			link: "#",
		},
		{
			text: "About",
			link: "#",
		},
		{
			text: "Contact",
			link: "#",
		},
		{
			text: "Reviews",
			link: "#",
		},
	];
</script>
