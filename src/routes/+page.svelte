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
			<button class="mt-5 md:mt-7 md:w-[91px] w-[70px] h-[25px] md:h-[36px] px-2 md:px-4 rounded-[4px] border border-b-[4px] border-[#4D4D4D] flex items-center justify-center outline-none gap-2 text-xs md:text-sm hover:cursor-pointer">Followed</button>
		</div>
		<div class="hidden w-[14%] text-right sm:flex flex-col justify-between">
			<div class="space-y-[1px]">
				<img src={company} alt="company icon" class="w-[25%] md:w-fit mr-0 ml-auto">
				<h2 class="text-xs sm:text-sm md:text-base font-semibold md:font-bold">Duggup</h2>
				<h4 class="text-[9px] md:text-xs text-[#7A9299]">Co-Founder and CEO</h4>
			</div>
			<div class="mt-3 flex items-center space-x-4">
				<a href="https://duggup.com" target="_blank" class="text-[9px] md:text-sm flex gap-1 items-center">My website <img src={visit} alt="visit my website option" class="w-[20%] md:w-fit"></a>
				<img src={more} alt="more options" class="w-[20%] md:w-fit hover:cursor-pointer">
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
		<div class="flex flex-wrap w-fit justify-center mx-auto mt-4 sm:mt-9 gap-2 sm:gap-4 xl:gap-9">
			<div class="w-[344px] border rounded-lg">
				<img src={stevej} alt="steve jobs' thumbnail" class="w-fit">
				<p class="px-1 sm:px-8 py-1 sm:py-4 text-xs md:text-sm">No amount of technology can convert a bad story into a good story.</p>
			</div>
			<div class="w-[344px] border rounded-lg">
				<img src={sama} alt="sam altman's thumbnail" class="w-fit rounded-t-xl">
				<p class="px-1 sm:px-8 py-1 sm:py-4 text-xs md:textsm">Most people don't have original ideas. Here is how Sam Altman pushes himself to have...</p>
			</div>
		</div>
	</div>
</div>

<!-- <div class="lg:w-[92%] xl:w-[83.3%] 2xl:w-[76.2%] my-0 mx-auto"> -->
<div class="ml-[3.2rem] sm:ml-[3.3rem] md:ml-[0.1rem] lg:ml-[3.2rem] my-0 mx-auto">
	<div class="flex gap-2 flex-row items-center">
		<img src={forward} alt="forward line" class="w-6 block md:hidden">
		<div class="flex flex-col w-[22%] sm:w-fit gap-1 md:text-right">
			<img src={company} alt="company logo" class="w-6 md:w-9 md:ml-auto">
			<h3 class="text-xs sm:text-sm md:text-base font-semibold md:font-bold">Duggup</h3>
			<span class="text-[9px] md:text-xs text-[#7A9299]">San Francisco Bay Area</span>
			<span class="text-[9px] md:text-xs text-[#7A9299]">Joined Nov 2023</span>
		</div>
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
		<div class="flex flex-wrap w-fit justify-center mx-auto sm:mt-9 gap-2 sm:gap-4 xl:gap-9">
			<div class="w-[344px] border rounded-lg">
				<img src={lessons} alt="startup lessons' thumbnail" class="w-fit">
				<p class="px-1 md:px-8 py-1 sm:py-4 text-xs md:textsm">Startup Lesson I am reflecting. Don't build for the "average person".</p>
			</div>
			<div class="w-[344px] border rounded-lg">
				<img src={regrets} alt="life regrets' thumbnail" class="w-fit rounded-t-xl">
				<p class="px-1 sm:px-8 py-1 sm:py-4 text-xs md:textsm">Your biggest regrets at 80 will be acts of omission.</p>
			</div>
		</div>
	</div>
</div>

<div class="ml-[3.2rem] sm:ml-[3.3rem] md:ml-[0.1rem] lg:ml-[3.2rem] my-0 mx-auto">
	<div class="flex gap-2 flex-row items-center">
		<img src={forward} alt="forward line" class="w-6 block md:hidden">
		<div class="flex flex-col w-[22%] sm:w-fit gap-1 md:text-right">
			<img src={betterup} alt="company logo" class="w-6 md:w-9 md:ml-auto">
			<h3 class="text-xs sm:text-sm md:text-base font-semibold md:font-bold">BetterUp</h3>
			<span class="text-[9px] md:text-xs text-[#7A9299]">San Francisco Bay Area</span>
			<span class="text-[9px] md:text-xs text-[#7A9299]">Joined
				Sep 2022</span>
		</div>
		<img src={forward} alt="forward line" class="w-6 hidden md:block">
		<div class="text-xs text-[#7A9299] w-fit ml-2 sm:ml-14">
			<h3 class="text-xs sm:text-sm md:text-xl font-semibold md:font-bold">VP Engineering</h3>
			<h5 class="text-[9px] md:text-xs text-[#7A9299]">Full-time</h5>
		</div>
	</div>
</div>

</div>