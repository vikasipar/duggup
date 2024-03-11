<script>
    export let companyImage;
    export let companyName;
    export let companyLocation;
    export let companyJoining;
</script>

<div class="flex flex-col w-[22%] sm:w-fit gap-1 md:text-right">
	<img src={companyImage} alt="company logo" class="w-6 md:w-9 md:ml-auto">
	<h3 class="text-xs sm:text-sm md:text-base font-semibold md:font-bold">{companyName}</h3>
	<span class="text-[9px] md:text-xs text-[#7A9299]">{companyLocation}</span>
	<span class="text-[9px] md:text-xs text-[#7A9299]">{companyJoining}</span>
</div>