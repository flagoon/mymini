<script>
	import { data } from '../data';
</script>

<h1>My Minis</h1>
<div class="flex flex-wrap justify-around sm:justify-between w-full gap-4">
	{#each data as { id, name, url, creator, previewUrl }}
		<div class="w-full sm:w-64 border-2 border-sky-400 p-2">
			<a href={`https://www.myminifactory.com/object/${url}`} class="flex flex-col"
				><img src={previewUrl} alt={name} />
				<h2 class="font-bold">{name}</h2></a
			>
		</div>
	{/each}
</div>
