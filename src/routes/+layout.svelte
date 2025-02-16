
<svelte:head>
   <title>Thierberger Schützen</title>
   <!-- <link rel="icon" type="image/svg" href={icon-path} /> -->
   <link rel="preload" as="font" href="../fonts/Typo-Speed-Bold-Italic-Demo.woff" type="font/woff" crossorigin="anonymous">
   <link rel="preload" as="font" href="../fonts/typo-speed-bold-italic-demo.woff2" type="font/woff2" crossorigin="anonymous">
   <link rel="preload" as="font" href="../fonts/Typo-Speed-Bold-Italic-Demo.eot" type="font/eot" crossorigin="anonymous"> 
   <link rel="preload" as="font" href="../fonts/Typo-Speed-Bold-Italic-Demo.otf" type="font/otf" crossorigin="anonymous"> 
   <link rel="preload" as="font" href="../fonts/Typo-Speed-Bold-Italic-Demo.svg" type="font/svg" crossorigin="anonymous"> 

 
 
</svelte:head>

<script lang='ts'>
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger, Dropdown, DropdownItem, DropdownDivider } from 'flowbite-svelte';
 	import { ChevronDownOutline, FacebookSolid, InstagramSolid } from 'flowbite-svelte-icons';
	import { page } from '$app/stores';
	import "../fonts/font-server.css"

	import "../app.css";

	import { Carousel } from 'flowbite-svelte';
	import { Footer, FooterBrand, FooterCopyright, FooterIcon, FooterLink, FooterLinkGroup } from 'flowbite-svelte';
	import { images } from '../imageData/+server';
	import Indicators from "flowbite-svelte/Indicators.svelte";

	let hideNavMenu = $state(true);

    const onNavHamburgerClick = (toggleFn: () => void) => {
        toggleFn();
        hideNavMenu = !hideNavMenu;
    };

    const onNavLinkClick = (toggleFn: () => void) => {
        hideNavMenu = true;
    };

let { children } = $props();
</script>


<div class="max-w-[90vw] m-auto">

	<Navbar let:toggle class="rounded-xl bg-gray-300 p-1 ">
		<NavHamburger onClick={() => onNavHamburgerClick(toggle)}  />
		<NavUl hidden={hideNavMenu}>
		  <NavLi class="md:hover:text-emerald-700" href="/" on:click={() => onNavLinkClick(toggle)}>Startseite</NavLi>
		  <NavLi class="md:hover:text-emerald-700" href="/calendar" on:click={() => onNavLinkClick(toggle)}>Termine</NavLi>
		  <NavLi class="cursor-pointer md:hover:text-emerald-700" >
			Über Uns<ChevronDownOutline class="w-6 h-6 ms-2 text-emerald-700 dark:text-white inline" />
		  </NavLi>
		  <Dropdown class="md:w-44 w-[80vw] z-20">
			<DropdownItem href="/about/gilde" on:click={() => onNavLinkClick(toggle)} >Gilde</DropdownItem>
			<DropdownItem href="/about/kompanie" on:click={() => onNavLinkClick(toggle)}>Kompanie</DropdownItem>
			<DropdownItem href="/about/ausschuss" on:click={() => onNavLinkClick(toggle)}>Ausschuss</DropdownItem>
			<DropdownItem href="/about/chronik" on:click={() => onNavLinkClick(toggle)}>Chronik</DropdownItem>
		  </Dropdown>
		  <NavLi class="cursor-pointer md:hover:text-emerald-700">
			Unser Schießstand<ChevronDownOutline class="w-6 h-6 ms-2 text-emerald-700 dark:text-white inline" />
		  </NavLi>
		  <Dropdown class="md:w-44 w-[80vw] z-20">
			<DropdownItem href="/schießstand/luftgewehr" on:click={() => onNavLinkClick(toggle)}>Luftgewehr</DropdownItem>
			<DropdownItem href="/schießstand/kleinkaliber" on:click={() => onNavLinkClick(toggle)}>Kleinkaliber</DropdownItem>
		  </Dropdown>
		  <NavLi class="md:hover:text-emerald-700" href="/beitritt" on:click={() => onNavLinkClick(toggle)}>Mitglied werden</NavLi>
		  <NavLi class="cursor-pointer md:hover:text-emerald-700">
			Der Thierberg Turm<ChevronDownOutline class="w-6 h-6 ms-2 text-emerald-700 dark:text-white inline " />
		  </NavLi>
		  <Dropdown class="md:w-44 w-[80vw] z-20">
			<DropdownItem href="/turm/informationen" on:click={() => onNavLinkClick(toggle)}>Zum Turm</DropdownItem>
			<DropdownItem href="/turm/geschichte" on:click={() => onNavLinkClick(toggle)}>Geschichte</DropdownItem>
		  </Dropdown>
		  <NavLi class="md:hover:text-emerald-700" href="/kontakt" on:click={() => onNavLinkClick(toggle)}>Kontakt</NavLi>
		</NavUl>
	  </Navbar>

	<div class="w-full z-0">
		<Carousel
			class=""
			style="height:25rem; z-index:0"
			{images} 
			duration="3000" 
			let:Indicators>

		</Carousel>
	</div>

	<div class="md:flex place-content-between -mt-[6rem] md:-mt-[7rem] z-40 relative">
		<div class="mb-4 rounded-xl bg-white py-3 px-3 mx-3 sm:w-[94%] md:w-auto">
			<a class="flex" title="Zur Startseite" href="/">
				<img class="md:w-24 w-20" alt="" src="/logoohnetextdunkelgruen.svg"/>
				<h1 class="typo_speed my-auto text-2xl font-extrabold leading-none tracking-tight  ml-4 md:text-3xl text-emerald-700 ">Thierberger<br>Schützen</h1>  
			</a>
		</div>
		<div class="mb-4 rounded-xl md:bg-white sm:bg-transparent w-max px-2 flex mr-3">
			<p class="m-auto font-semibold">Unterstützt<br>durch:</p>
			<img class="w-12 mx-5 my-5" alt="Pirlo" src="https://www.pirlo.com/build/pirlo/images/template/logo.svg"/>
			<img class="w-20 mx-2 my-5" alt="Stadt Kufstein" src="https://upload.wikimedia.org/wikipedia/commons/7/79/Kufstein_Logo.svg"/>
		</div>
	</div>

{@render children()}

<Footer class="px-8 py-4">
	<div class="sm:flex sm:items-center sm:justify-between">
	<FooterCopyright copyrightMessage="" by="Thierberger Schützen, Morsbach 71 6330 Kufstein, ZVR-Nr.: 262203066" year={2025} />
	<FooterLinkGroup ulClass="flex flex-wrap justify-center items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0">
	  <FooterLink href="https://maps.app.goo.gl/skP2fuyF4s461QY9A" target="_blank">Anfahrt</FooterLink>
	  <FooterLink href="/impressum">Impressum</FooterLink>
	  <FooterLink href="/datenschutz">Datenschutz</FooterLink>
	</FooterLinkGroup>

	 
	<FooterLinkGroup ulClass="flex flex-wrap justify-center items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0">
  
	  <FooterIcon class="p-2" href="https://www.instagram.com/thierberger.schuetzen/" target="_blank">
        <InstagramSolid class="w-7 h-7 text-gray-500 dark:text-gray-500 hover:text-gray-900 dark:hover:text-white" />
      </FooterIcon>
	  <FooterIcon class="p-2 " href="https://www.facebook.com/p/Thierberger-Schützen-100057561487417/" target="_blank">
        <FacebookSolid class="w-6 h-6 text-gray-500 dark:text-gray-500 hover:text-gray-900 dark:hover:text-white" />
      </FooterIcon>
	</FooterLinkGroup>
	</div>
  </Footer>

</div>


<style>
	

	.typo_speed{
		font-family: 'Typo-Speed-Bold-Italic-Demo';
		}


/* .test{
	background-color: red;
} */
</style>

