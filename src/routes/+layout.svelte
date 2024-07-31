<script>
	import '../app.css';
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger, ImagePlaceholder, Skeleton, TextPlaceholder } from 'flowbite-svelte';

</script>
  
<div class="relative px-8" style="padding-top: 4rem">
	<Navbar class="px-2 sm:px-4 py-2.5 fixed w-full z-20 top-0 start-0 border-b">
		<NavBrand href="/">
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Portfolio</span>
		</NavBrand>
		<NavHamburger />
		<NavUl>
		<NavLi href="/" active={true}>Home</NavLi>
		<NavLi href="/about">About</NavLi>
		<NavLi href="/docs/components/navbar">Navbar</NavLi>
		<NavLi href="/pricing">Pricing</NavLi>
		<NavLi href="/contact">Contact</NavLi>
		</NavUl>
	</Navbar>
</div>
<slot></slot>
