
<svelte:head>
   <title>Thierberger Schützen</title>
   <!-- <link rel="icon" type="image/svg" href={icon-path} /> -->
</svelte:head>

<script>
import { Navbar, NavBrand, NavLi, NavUl, NavHamburger, Dropdown, DropdownItem, DropdownDivider } from 'flowbite-svelte';
  import { ChevronDownOutline } from 'flowbite-svelte-icons';
  import { page } from '$app/stores';


import "../app.css";

import { Carousel } from 'flowbite-svelte';
import { images } from '../imageData/+server';
import Indicators from "flowbite-svelte/Indicators.svelte";

let { children } = $props();
</script>


<div class="max-w-[90vw] m-auto">
<div class="w-full z-0">
	<Carousel
		class=""
		style="height:25rem; z-index:0"
		{images} 
		duration="3000" 
		let:Indicators>

	</Carousel>
  </div>

<div class="flex place-content-between -mt-20 z-40 relative">
	<div class="mb-4 rounded-xl bg-white w-max py-3 px-3 ml-3 flex">
		  <img alt="" src="https://placehold.co/50x50"/>
		  <h1 class="text-4xl font-extrabold leading-none tracking-tight md:text-5xl text-emerald-700 ">Thierberger Schützen</h1>  
	</div>
	<div class="mb-4 rounded-xl bg-white w-max px-2 flex mr-3">
		<p class="m-auto font-semibold">Unterstützt durch:</p>
		<img class="max-w-20 mx-1" alt="Pirlo" src="https://www.pirlo.com/build/pirlo/images/template/logo.svg"/>
		<img class="max-w-20 mx-1" alt="Stadt Kufstein" src="https://upload.wikimedia.org/wikipedia/commons/7/79/Kufstein_Logo.svg"/>
	</div>
</div>

  <Navbar class="rounded-xl bg-gray-300 p-1">
	<NavHamburger />
	<NavUl>
	  <NavLi class="md:hover:text-emerald-700" href="/">Startseite</NavLi>
	  <NavLi class="md:hover:text-emerald-700" href="/calendar">Termine</NavLi>
	  <NavLi class="cursor-pointer md:hover:text-emerald-700">
		Über Uns<ChevronDownOutline class="w-6 h-6 ms-2 text-emerald-700 dark:text-white inline" />
	  </NavLi>
	  <Dropdown class="w-44 z-20">
		<DropdownItem href="/about/gilde">Gilde</DropdownItem>
		<DropdownItem href="/about/kompanie">Kompanie</DropdownItem>
		<DropdownItem href="/about/ausschuss">Ausschuss</DropdownItem>
		<DropdownItem href="/about/chronik">Chronik</DropdownItem>
	  </Dropdown>
	  <NavLi class="cursor-pointer md:hover:text-emerald-700">
		Unser Schießstand<ChevronDownOutline class="w-6 h-6 ms-2 text-emerald-700 dark:text-white inline" />
	  </NavLi>
	  <Dropdown class="w-44 z-20">
		<DropdownItem href="/schießstand/luftgewehr">Luftgewehr</DropdownItem>
		<DropdownItem href="/schießstand/kleinkaliber">Kleinkaliber</DropdownItem>
	  </Dropdown>
	  <NavLi class="md:hover:text-emerald-700" href="/beitritt">Mitglied werden</NavLi>
	  <NavLi class="cursor-pointer md:hover:text-emerald-700">
		Der Thierberg Turm<ChevronDownOutline class="w-6 h-6 ms-2 text-emerald-700 dark:text-white inline " />
	  </NavLi>
	  <Dropdown class="w-44 z-20">
		<DropdownItem href="/turm/informationen">Zum Turm</DropdownItem>
		<DropdownItem href="/schießstand/kleinkaliber">Geschichte</DropdownItem>
	  </Dropdown>
	  <NavLi class="md:hover:text-emerald-700" href="/kontakt">Kontakt</NavLi>
	</NavUl>
  </Navbar>
{@render children()}

</div>


<style>


/* .test{
	background-color: red;
} */
</style>

