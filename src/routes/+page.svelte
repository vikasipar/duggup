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
<section class="w-[80%] mx-auto mt-9">
	<div class="flex flex-row flex-wrap justify-between items-center">
		<div class="w-[14%]">
			<img src={profile} alt="user profile" class="w-fit">
			<h1 class="text-2xl font-bold text-[#4B5C6D] text-center">Krishna Kiran</h1>
		</div>
		<div class="w-[60%] px-11 text-sm">
			<p class="">Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of Engineering. I write hot-takes on building a business, shipping delightful products and accelerating product and career growth.</p>
			<button class="mt-7 w-[91px] h-[36px] px-4 rounded-[4px] border border-b-[4px] border-[#4D4D4D] flex items-center justify-center outline-none gap-2 text-sm hover:cursor-pointer">Followed</button>
		</div>
		<div class="w-[14%] text-right flex flex-col justify-between">
			<div class="space-y-[1px]">
				<img src={company} alt="company icon" class="w-fit mr-0 ml-auto">
				<h2 class="text-base font-bold">Duggup</h2>
				<h4 class="text-xs text-[#7A9299]">Co-Founder and CEO</h4>
			</div>
			<div class="mt-3 flex items-center space-x-4">
				<a href="www.duggup.com" target="_blank" class="text-sm flex gap-1 items-center">My website <img src={visit} alt="visit my website option" class="w-fit"></a>
				<img src={more} alt="more options" class="w-fit hover:cursor-pointer">
			</div>
		</div>
	</div>	
</section>


<div class="w-[80%] mx-auto text-[14px] my-0">
	<div class="flex flex-row flex-wrap items-center gap-11 ">
		<div class="w-fit flex items-center">
			<p class="text-xs text-[#7A9299]">Dec 2023</p>
			<img src={progress} alt="progress line" class="w-fit">
		</div>
		<div class="w-[344px] border rounded-lg">
			<img src={stevej} alt="steve jobs' thumbnail" class="w-fit">
			<p class="px-8 py-4">No amount of technology can convert a bad story into a good story.</p>
		</div>
		<div class="w-[344px] border rounded-lg">
			<img src={sama} alt="sam altman's thumbnail" class="w-fit rounded-t-xl">
			<p class="px-8 py-4">Most people don't have original ideas. Here is how Sam Altman pushes himself to have...</p>
		</div>
	</div>
</div>

<div class="w-[92%] my-0 mx-auto">
	<div class="flex gap-2 flex-row flex-wrap items-center">
		<div class="flex flex-col w-fit gap-1 text-right">
			<img src={company} alt="company logo" class="w-9 ml-auto">
			<h3 class="text-base font-bold">Duggup</h3>
			<span class="text-xs text-[#7A9299]">San Francisco Bay Area</span>
			<span class="text-xs text-[#7A9299]">Joined Nov 2023</span>
		</div>
		<img src={forward} alt="forward line" class="w-6">
		<div class="text-xs text-[#7A9299] w-fit ml-14">
			<h3 class="text-xl font-bold">Co-Founder and CEO</h3>
			<h5 class="text-xs text-[#7A9299]">Full-time · Remote</h5>
		</div>
	</div>
</div>

<div class="w-[80%] mx-auto text-[14px]">
	<div class="flex flex-row flex-wrap items-center gap-11 ">
		<div class="w-fit flex items-center">
			<p class="text-xs text-[#7A9299]">Dec 2023</p>
			<img src={progress} alt="progress line" class="w-fit">
		</div>
		<div class="w-[344px] border rounded-lg">
			<img src={lessons} alt="startup lessons' thumbnail" class="w-fit">
			<p class="px-8 py-4">Startup Lesson I am reflecting. Don't build for the "average person".</p>
		</div>
		<div class="w-[344px] border rounded-lg">
			<img src={regrets} alt="life regrets' thumbnail" class="w-fit rounded-t-xl">
			<p class="px-8 py-4">Your biggest regrets at 80 will be acts of omission.</p>
		</div>
	</div>
</div>

<div class="w-[92%] my-0 mx-auto">
	<div class="flex gap-2 flex-row flex-wrap items-center">
		<div class="flex flex-col w-fit gap-1 text-right">
			<img src={betterup} alt="company logo" class="w-9 ml-auto">
			<h3 class="text-base font-bold">BetterUp</h3>
			<span class="text-xs text-[#7A9299]">San Francisco Bay Area</span>
			<span class="text-xs text-[#7A9299]">Joined
				Sep 2022</span>
		</div>
		<img src={forward} alt="forward line" class="w-6">
		<div class="text-xs text-[#7A9299] w-fit ml-14">
			<h3 class="text-xl font-bold">VP Engineering</h3>
			<h5 class="text-xs text-[#7A9299]">Full-time</h5>
		</div>
	</div>
</div>

</div>