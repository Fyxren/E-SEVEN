<script lang="ts">
	type IMember = {
		name: string;
		description: string;
		image: string;
	};
	export let member: IMember;
</script>

<div>
	<img
		src={member.image}
		alt={`image ${member.name}`}
		class="object-contain duration-300 rounded-lg shadow-xl saturate-50 hover:saturate-100"
	/>
	<h3 class="mt-2 text-4xl font-thin tracking-wide">{member.name}</h3>
	<p>{member.description}</p>
</div>
