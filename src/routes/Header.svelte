<script>
	import logo from '$lib/images/duggup-logo.svg';
	import profile from '$lib/images/profile.png';
	import home from '$lib/images/home.png';
	import explore from '$lib/images/explore.png';
	import learn from '$lib/images/learn.png';
	import post from '$lib/images/post.png';
	import down from '$lib/images/down.png';
	import logout from '$lib/images/logout.png';
	import settings from '$lib/images/settings.png';

	let options = false;
</script>

<header class="sticky top-0 z-50 flex h-16 w-full items-center px-[16px] border-b border-[#525C69]/30 border-dotted backdrop-blur">
	<div class="text-xl">
		<a href="/" class="flex justify-start gap-2 w-fit">
			<img src={logo} alt="Duggup Logo" class="w-fit"/>
			<h2 class="text-[#020817] font-semibold">duggup</h2>
		</a>
	</div>

	<nav class="flex items-center text-sm font-[400] text-[#020817]">
		<div class="flex">
			<span class="min-w-[102px] text-center px-4 py-2 rounded-[4px] border-white border border-b-[4px] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
				<img src={home} alt="home icon" class="w-fit">
				Home
			</span>
			<span class="min-w-[102px] text-center px-4 py-2 rounded-[4px] border-white border border-b-[4px] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
				<img src={explore} alt="explore icon" class="w-fit">
				Explore
			</span>
			<span class="min-w-[102px] text-center px-4 py-2 rounded-[4px] border-white border border-b-[4px] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
				<img src={learn} alt="learn icon" class="w-fit">
				Learn
			</span>
			<span class="min-w-[102px] px-4 rounded-[4px] mx-5 border border-b-[4px] border-[#4D4D4D] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
				<img src={post} alt="post icon" class="w-fit">
				Post<span class="w-1"></span>
			</span>
		</div>
		<div class="w-[272px] ml-2">
			<div role="button" tabindex="0" class="text-center flex items-center justify-center cursor-pointer gap-[8px]" on:click={() => options=(!options)} on:keydown={(e)=> {if(e.key === "Enter" || e.key === " "){options=(!options);}}}>
				<img src={profile} alt="user profile" class="w-9 p-[0.5px] border-[0.7px] rounded-full border-[#4d4d4d]">
				<h3 class="font-[500] text-lg">Krishna Kiran</h3>
				<img src={down} alt="down arrow icon" class="w-fit">
			</div>
			{#if (options)}
				<div class="absolute z-50 w-[212px] top-[70px] shadow-md h-24 pt-[5px] border rounded right-2">
					<span class="w-[95%] mx-auto text-center px-1 py-2 rounded-[4px] hover:bg-[#ebf3fa] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
						<img src={settings} alt="settings icon" class="w-5 opacity-60">
						Settings
					</span>
					<span class="w-[90%] mx-auto text-center px-1 py-2 rounded-[4px] hover:bg-[#ebf3fa] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
						<img src={logout} alt="logout icon" class="w-[18px] opacity-80">
						Logout
					</span>
				</div>
			{/if}
		</div>
	</nav>

</header>
