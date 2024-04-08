<script>
	import {
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
		// @ts-ignore
		ImagePlaceholder,
		// @ts-ignore
		Skeleton,
		// @ts-ignore
		TextPlaceholder
	// @ts-ignore
	} from 'flowbite-svelte';
</script>

<div class="relative px-8">
	<Navbar class="px-2 sm:px-4 py-2.5 fixed w-full z-20 top-0 start-0 border-b">
		<NavBrand href="/">
			<span class="self-center whitespace-nowrap text-3xl font-semibold dark:text-white text-purple-700"
				>OpenDataMalawi</span
			>
		</NavBrand>
		<NavHamburger class="bg-gray-50"/>
		<NavUl class="rounded">
			<NavLi href="/" active={true}>Home</NavLi>
			<NavLi href="/datasets">Explore Datasets</NavLi>
			<NavLi href="/contributions">Contributions</NavLi>
			<NavLi href="/analytics">Analytics</NavLi>
			<NavLi href="/contact">Contact  Us</NavLi>
		</NavUl>
	</Navbar>
</div>
