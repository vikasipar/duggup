<script>
	import profile from '$lib/images/user.png';
	import company from '$lib/images/company.png';
	import visit from '$lib/images/visit.png';
	import more from '$lib/images/more.png';
	import progress from '$lib/images/progress.png';
	import stevej from '$lib/images/stevej.png';
	import sama from '$lib/images/sama.png';
	import betterup from '$lib/images/betterup.png';
	import regrets from '$lib/images/regrets.png';
	import lessons from '$lib/images/lessons.png';
	import forward from '$lib/images/forward.png';
	import {M} from 'svelte-motion';
	import Card from '../components/Card.svelte';
	import Company from '../components/Company.svelte';
</script>

<svelte:head>
	<title>Duggup</title>
	<meta name="description" content="Duggup social media app" />
</svelte:head>	

<div class="w-[98vw] mx-auto">
<section class="w-[90%] lg:w-[80%] 2xl:w-[70%] mx-auto mt-9 lg:mt-16">
	<div class="flex flex-row flex-wrap justify-between items-center">
		<div class="w-[30%] sm:w-[14%]">
			<img src={profile} alt="user profile" class="w-[70%] mx-auto sm:w-fit">
			<h1 class="text-sm sm:text-base md:text-2xl font-semibold md:font-bold text-[#4B5C6D] text-center">Krishna Kiran</h1>
		</div>
		<div class="w-[40%] sm:w-[14%] text-right flex sm:hidden flex-col justify-between">
			<div class="space-y-[1px]">
				<img src={company} alt="company icon" class="w-[20%] sm:w-[25%] md:w-fit mr-0 ml-auto">
				<h2 class="text-xs sm:text-sm md:text-base font-semibold md:font-bold">Duggup</h2>
				<h4 class="text-[9px] md:text-xs text-[#7A9299]">Co-Founder and CEO</h4>
			</div>
			<div class="w-[65%] ml-auto sm:w-[99%] mt-1 sm:mt-3 flex items-center space-x-4">
				<a href="https://duggup.com" target="_blank" class="text-[8px] md:text-sm flex gap-1 items-center">My website <img src={visit} alt="visit my website option" class="w-[11%] sm:w-[20%] md:w-fit"></a>
				<img src={more} alt="more options" class="w-[12%] sm:w-[20%] md:w-fit hover:cursor-pointer">
			</div>
		</div>
		<div class="w-full sm:w-[70%] mt-2 sm:mt-0 text-justify lg:text-left lg:w-[60%] px-3 sm:px-11 text-xs md:text-sm">
			<p class="">Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of Engineering. I write hot-takes on building a business, shipping delightful products and accelerating product and career growth.</p>
			<M.button 
			initial={{scale: 0.8}}
		    animate={{scale: 1}}
		    transition={{duration:0.9}}
			class="mt-5 md:mt-7 md:w-[91px] w-[70px] h-[25px] md:h-[36px] px-2 md:px-4 rounded-[4px] border border-b-[4px] border-[#4D4D4D] flex items-center justify-center outline-none gap-2 text-xs md:text-sm hover:cursor-pointer">Followed</M.button>
		</div>
		<div class="hidden w-[14%] text-right sm:flex flex-col justify-between">
			<div class="space-y-[1px]">
				<img src={company} alt="company icon" class="w-[25%] md:w-fit mr-0 ml-auto">
				<h2 class="text-xs sm:text-sm md:text-base font-semibold md:font-bold">Duggup</h2>
				<h4 class="text-[9px] md:text-xs text-[#7A9299]">Co-Founder and CEO</h4>
			</div>
			<div class="mt-3 flex items-center space-x-4">
				<M.a 
				initial={{scale: 1}}
				whileHover={{scale: 1.03}}
				transition={{duration:0.4}}
				href="https://duggup.com" target="_blank" class="text-[9px] md:text-sm flex gap-1 items-center">My website <img src={visit} alt="visit my website option" class="w-[20%] md:w-fit"></M.a>
				<img src={more} alt="more options" class="w-[20%] md:w-fit hover:cursor-pointer hover:animate-bounce hover:rotate-12">
			</div>
		</div>
	</div>	
</section>


<div class="w-[80%] 2xl:w-[70%] mx-auto text-[14px] my-0">
	<div class="flex flex-row items-center gap-12">
		<div class="w-fit flex items-center">
			<p class="text-xs text-[#7A9299]">Dec 2023</p>
			<img src={progress} alt="progress line" class="w-fit">
		</div>
		<M.div 
		initial={{scale: 0.9}}
		animate={{scale: 1}}
		transition={{duration:0.9}}
		class="posts flex flex-wrap sm:overflow-visible w-fit justify-center mx-auto mt-4 sm:mt-9 gap-2 sm:gap-4 xl:gap-9">
		    <Card img={stevej} paragraph={"No amount of technology can convert a bad story into a good story."}/>
		    <Card img={sama} paragraph={"Most people don't have original ideas. Here is how Sam Altman pushes himself to have..."}/>
		</M.div>
	</div>
</div>

<div class="ml-[3.2rem] sm:ml-[3.3rem] md:ml-[0.1rem] lg:ml-[3.2rem] my-0 mx-auto">
	<div class="flex gap-2 flex-row items-center">
		<img src={forward} alt="forward line" class="w-6 block md:hidden">
		<Company companyImage={company} companyName={"Duggup"} companyLocation={"San Francisco Bay Area"} companyJoining={"Joined Nov 2023"}/>
		<img src={forward} alt="forward line" class="w-6 hidden md:block">
		<div class="text-xs text-[#7A9299] w-fit ml-2 md:ml-14">
			<h3 class="text-xs sm:text-sm md:text-xl font-semibold md:font-bold">Co-Founder and CEO</h3>
			<h5 class="text-[9px] md:text-xs text-[#7A9299]">Full-time · Remote</h5>
		</div>
	</div>
</div>

<div class="w-[80%] 2xl:w-[70%] mx-auto text-[14px]">
	<div class="flex flex-row items-center gap-11 ">
		<div class="w-fit flex items-center">
			<p class="text-xs text-[#7A9299]">Dec 2023</p>
			<img src={progress} alt="progress line" class="w-fit">
		</div>
		<M.div
		initial={{scale: 0.9}}
		animate={{scale: 1}}
		transition={{duration:0.9}}
		class="flex flex-wrap w-fit sm:overflow-visible justify-center mx-auto sm:mt-9 gap-2 sm:gap-4 xl:gap-9">
		    <Card img={lessons} paragraph={"Startup Lesson I am reflecting. Don't build for the average person."}/>
		    <Card img={regrets} paragraph={"Your biggest regrets at 80 will be acts of omission."}/>
		</M.div>
	</div>
</div>

<div class="ml-[3.2rem] sm:ml-[3.3rem] md:ml-[0.1rem] lg:ml-[3.2rem] my-0 mx-auto">
	<div class="flex gap-2 flex-row items-center">
		<img src={forward} alt="forward line" class="w-6 block md:hidden">
		<Company companyImage={betterup} companyName={"BetterUp"} companyLocation={"San Francisco Bay Area"} companyJoining={"Joined Sep 2022"}/>
		<img src={forward} alt="forward line" class="w-6 hidden md:block">
		<div class="text-xs text-[#7A9299] w-fit ml-2 sm:ml-14">
			<h3 class="text-xs sm:text-sm md:text-xl font-semibold md:font-bold">VP Engineering</h3>
			<h5 class="text-[9px] md:text-xs text-[#7A9299]">Full-time</h5>
		</div>
	</div>
</div>

</div>

<style>
	div::-webkit-scrollbar {
  display: none;
}
</style>