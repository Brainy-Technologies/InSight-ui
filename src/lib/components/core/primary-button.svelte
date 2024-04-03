<script lang="ts">
	import type { ButtonColor, ColorMap } from '$lib/types';

	export let text: string = '';
	export let color: ButtonColor = 'primary';

	const mapping: Array<ColorMap> = [
		{
			name: 'primary',
			color: 'indigo'
		},
        {
            name: 'secondary',
            color: 'sky'
        },
		{
			name: 'success',
			color: 'emerald'
		},
		{
			name: 'error',
			color: 'red'
		},
		{
			name: 'warning',
			color: 'yellow'
		},
		{
			name: 'link',
			color: 'sky'
		}
	];

	$: finalColorClass = `bg-${(mapping.find((mapp: ColorMap) => mapp.name === color)?.color || 'gray')}-600`;
</script>

<button class={finalColorClass + "text-white px-4 py-1.5"}>
	{text}
</button>

<style scoped lang="scss">
</style>
