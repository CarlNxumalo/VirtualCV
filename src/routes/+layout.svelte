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
		<NavLi href="#MySkills">Skills</NavLi>
		<NavLi href="#MyStack">Stack</NavLi>
		<NavLi href="#MyProjects">Projects</NavLi>
		<NavLi href="#MyEducation">Education</NavLi>
		<NavLi href="#MyAbout">About</NavLi>
		</NavUl>
	</Navbar>
</div>
<slot></slot>
