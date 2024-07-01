<script>
	import { data } from '../data';
</script>

<h1>My Minis</h1>
<div class="flex flex-wrap gap-4">
	{#each data as { id, name, url, creator, previewUrl }}
		<div class="w-1/6 border-2 border-sky-400 p-2 min-h-24">
			<a href={`https://www.myminifactory.com/object/${url}`} class="flex flex-col"
				><img src={previewUrl} alt={name} />
				<h2 class="font-bold">{name}</h2></a
			>
		</div>
	{/each}
</div>
