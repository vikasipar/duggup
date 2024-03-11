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
	import menu from '$lib/images/menu.png';
	import close from '$lib/images/close.png';

	let options = false;
</script>

<header class="sticky top-0 z-50 h-16 w-full flex justify-between items-center px-4 border-b border-[#525C69]/30 border-dotted backdrop-blur">
	<span role="button" tabindex="0" class="block md:hidden w-fit" on:click={() => options=(!options)} on:keydown={(e)=> {if(e.key === "Enter" || e.key === " "){options=(!options);}}}>
		{#if (options)}
		<img src={close} alt="close menu icon" class="w-7">		
		{:else}
		<img src={menu} alt="hamburger menu icon" class="w-7">
		{/if}
	</span>

	<div class="text-xl w-fit">
		<a href="/" class="flex justify-start gap-2 w-fit">
			<img src={logo} alt="Duggup Logo" class="w-fit md:w-11"/>
			<h2 class="text-[#020817] font-semibold">duggup</h2>
		</a>
	</div>

	<nav class="flex max-w-fit items-center text-sm font-[400] text-[#020817]">
		<div class="hidden md:flex">
			<span class="w-[110px] text-center px-2 rounded-[4px] border-transparent border border-b-[4px] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
				<img src={home} alt="home icon" class="w-fit">
				Home
			</span>
			<span class="w-[110px] text-center px-2 py-2 rounded-[4px] border-transparent border border-b-[4px] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
				<img src={explore} alt="explore icon" class="w-fit">
				Explore
			</span>
			<span class="w-[110px] text-center px-2 py-2 rounded-[4px] border-transparent border border-b-[4px] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
				<img src={learn} alt="learn icon" class="w-fit">
				Learn
			</span>
			<span class="max-w-[102px] px-4 rounded-[4px] mx-5 border border-b-[4px] border-[#4D4D4D] flex items-center justify-center outline-none gap-2 hover:cursor-pointer">
				<img src={post} alt="post icon" class="w-fit">
				Post<span class="w-1"></span>
			</span>
		</div>
		<div class="min-w-fit max-w-[202px] ml-2">
			<div role="button" tabindex="0" class="text-center z-[100] flex items-center justify-center cursor-pointer gap-[8px]" on:click={() => options=(!options)} on:keydown={(e)=> {if(e.key === "Enter" || e.key === " "){options=(!options);}}}>
				<img src={profile} alt="user profile" class="w-fit md:w-12 p-[0.5px] border-[0.7px] rounded-full border-[#4d4d4d]">
				<h3 class="font-[500] text-lg hidden sm:block">Krishna Kiran</h3>
				{#if (!options)}
				<img src={down} alt="down arrow icon" class="w-6 hidden md:block">
				{:else}
				<img src={down} alt="down arrow icon" class="w-6 hidden md:block rotate-180">
				{/if}
			</div>
		</div>
	</nav>

</header>
{#if (options)}
	<div class="hidden md:block options absolute z-[100] w-[212px] top-[70px] shadow-md h-24 pt-[5px] border rounded right-2">
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

{#if (options)}
<div class="navbar flex md:hidden flex-col justify-center items-center gap-3 z-[100] bg-white h-svh w-screen absolute">
	<span class="w-[110px] text-center px-2 py-2 rounded-[4px] border-transparent border border-b-[4px] flex items-center justify-start bg-inherit outline-none gap-2 hover:cursor-pointer">
		<img src={home} alt="home icon" class="w-7 bg-inherit">
		Home
	</span>
	<span class="w-[110px] text-center px-2 py-2 rounded-[4px] border-transparent border border-b-[4px] flex items-center justify-start bg-inherit outline-none gap-2 hover:cursor-pointer">
		<img src={explore} alt="explore icon" class="w-7 bg-inherit">
		Explore
	</span>
	<span class="w-[110px] text-center px-2 py-2 rounded-[4px] border-white border border-b-[4px] flex items-center justify-start outline-none gap-2 hover:cursor-pointer bg-inherit">
		<img src={learn} alt="learn icon" class="w-7 bg-inherit">
		Learn
	</span>
	<span class="w-[110px] text-center px-2 py-2 rounded-[4px] border-transparent border border-b-[4px] flex items-center justify-start outline-none gap-2 hover:cursor-pointer bg-inherit">
		<img src={post} alt="post icon" class="w-7 bg-inherit">
		Post<span class="w-1"></span>
	</span>
	<span class="w-[110px] text-center px-2 py-2 rounded-[4px] flex items-center justify-start outline-none gap-2 hover:cursor-pointer bg-inherit">
		<img src={settings} alt="settings icon" class="w-[20%] opacity-60 bg-inherit">
		Settings
	</span>
	<span class="w-[110px] text-center px-2 py-2 rounded-[4px] flex items-center justify-start outline-none gap-2 hover:cursor-pointer bg-inherit">
		<img src={logout} alt="logout icon" class="w-[20%] opacity-80 bg-inherit">
		Logout
	</span>
</div>
{/if}

<style>
	.options{
		animation: op 0.6s;
	}
	@keyframes op{
		0%{transform: translateY(-55px); opacity: 0;}
		50%{opacity: 0;}
		100%{transform: translateY(0); opacity: 1;}
	}

	.navbar{
		animation: nav 1s;
	}
	@keyframes nav{
		0%{transform: translateX(-555px);}
		100%{transform: translateX(0);}
	}
</style>
