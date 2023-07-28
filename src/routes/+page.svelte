<script lang="ts">
	import MemberCard from '$lib/components/MemberCard.svelte';
	import RT from '$lib/components/RegionText.svelte';
	import members from '../data/members';
</script>

<main class="my-16 space-y-24">
	<!-- Header -->
	<div class="grid grid-cols-2 gap-20">
		<iframe
			src="https://www.youtube-nocookie.com/embed/681juG4vjkI?controls=0"
			title="YouTube video player"
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
			allowfullscreen
			color="#596655"
			class="w-full rounded-lg shadow-lg h-max aspect-video"
		/>
		<div class="flex flex-col justify-around">
			<div>
				<h1 class="text-6xl font-thin">Wij zijn <span class="font-normal">E-SEVEN</span></h1>
				<p class="mt-2 text-2xl">Drie vrienden die al jaren muziek maken.</p>
				<div class="mt-5 space-y-2">
					<p>
						Wij spelen graag op bruiloften of andere evenementen! Ons repetoire is gevarieerd: van
						dansmuziek tot ballads en van Nederlandstalig tot eighties.
					</p>
					<p>
						We zijn actief in de regio
						<RT region="zwolle" />,
						<RT region="kampen" />,
						<RT region="elburg" />, en <RT region="nunspeet" />
						✨️
					</p>
				</div>
			</div>
			<a href="/contact" class="shadow-lg btn btn-primary btn-wide">Contact</a>
		</div>
	</div>

	<!-- Members -->
	<div class="grid grid-cols-3 gap-32">
		{#each members as x}
			<MemberCard member={x} />
		{/each}
	</div>

	<!-- CTA -->
	<div class="flex flex-col justify-center text-center">
		<h2 class="text-4xl font-bold tracking-wider">
			Binnenkort een <span class="text-primary">bruiloft</span> of een ander
			<span class="text-primary">evenement</span>?
		</h2>

		<div class="grid self-center grid-cols-4 gap-16 mt-10 max-w-7xl">
			<div
				class="flex flex-col items-center justify-center w-48 gap-5 px-5 py-10 duration-300 border-4 rounded-lg hover:scale-110 hover:rotate-3 border-secondary"
			>
				<p class="text-6xl duration-300">💕</p>
				<p>3 vrienden die al jaren samen muziek maken</p>
			</div>
			<div
				class="flex flex-col items-center justify-center w-48 gap-5 px-5 py-10 duration-300 border-4 rounded-lg hover:scale-110 hover:rotate-3 border-secondary"
			>
				<p class="text-6xl duration-300">✨️</p>
				<p>Gevarieerd repetoire</p>
			</div>
			<div
				class="flex flex-col items-center justify-center w-48 gap-5 px-5 py-10 duration-300 border-4 rounded-lg hover:scale-110 hover:rotate-3 border-secondary"
			>
				<p class="text-6xl duration-300">🎶</p>
				<p>Actief in in de regio Zwolle, Kampen, Elburg en Nunspeet</p>
			</div>
			<div
				class="flex flex-col items-center justify-center w-48 gap-5 px-5 py-10 duration-300 border-4 rounded-lg hover:scale-110 hover:rotate-3 border-secondary"
			>
				<p class="text-6xl duration-300">🎤</p>
				<p>Akoestisch of full band</p>
			</div>
		</div>
		<a href="/contact" class="self-center mt-10 shadow-lg btn btn-primary btn-wide"
			>Neem contact op</a
		>
	</div>
</main>
