<script lang="ts">
	import type { Opis } from './types';

	// export let name: string;
	// export let image: string;
	// export let description: string;

	export let opis: Opis;

	// const name = opis.name;
	// const image = opis.image;
	// const description = opis.description;

	// tole spodaj je enako kot tri vrstice nad tem - ampak v krajši obliki;
	const { name, image, description } = opis;
</script>

<div class="p-5 rounded-2xl border-4 border-black bg-gradient-to-r from-green-600 to bg-purple-700">
	<h4 class="text-3xl">{name.toUpperCase()}</h4>

	<img src={image} />
	<p>{description}</p>
	<button class="bg-blue-950 hover:bg-blue-900 text-white rounded-xl p-2">Preberi več</button>
</div>
