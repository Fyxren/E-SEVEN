<script lang="ts">
	import RT from '$lib/components/RegionText.svelte';
</script>

<main class="mt-24">
	<div class="grid grid-cols-2 gap-20">
		<iframe
			src="https://www.youtube-nocookie.com/embed/681juG4vjkI?controls=0"
			title="YouTube video player"
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
			allowfullscreen
			color="#596655"
			class="rounded-lg w-full h-max aspect-video"
		/>
		<div class="flex flex-col justify-around">
			<div>
				<h1 class="text-6xl font-thin">Wij zijn <span class="font-normal">E-SEVEN</span></h1>
				<p class="text-2xl mt-2">Drie vrienden die al jaren muziek maken.</p>
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
			<a href="/contact" class="btn btn-primary btn-wide">Contact</a>
		</div>
	</div>
</main>
