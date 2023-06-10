<script setup>
import Card from "./components/Card.vue";
</script>
<template>
	<div class=" mx-16 mt-8 p-8 rounded-lg bg-slate-50">
		<h1 class="text-5xl font-mono font-extrabold text-gradient bg-clip-text text-transparent">elexn.uk/</h1>
		<p class="text-lg">
			Elexn UK is a collection of web apps and tools around United Kingdom politics and elections. Source code for all projects are available on <a href="https://github.com/elexnuk" target="_blank" class=" text-cyan-500 visited:text-purple-500 underline">Github</a>. Suggestions/Contributions are welcome.
		</p>
		<div class="bg-slate-100 p-4 mx-4 mt-2 rounded-lg flex flex-row gap-4 flex-wrap">
			<Card url="https://councils.elexn.uk/" name="Councils" description="Council Colouring. Colour maps of council wards."></Card>
			<Card url="https://arches.elexn.uk/" name="Arches" description="Parliament Diagram Creator. Currently only supports Arches."></Card>
			<Card url="https://elections.elexn.uk/" name="Elections" description="National and By-Election Result Viewer"></Card>
			<Card url="https://petitions.elexn.uk/" name="Petitions" description="Parliament Petition data viewer."></Card>
		</div>

		<h1 class="text-5xl font-sans font-thin">External</h1>
		<p class="text-lg">
			Some other useful apps and tools:
		</p>
		<div class="bg-slate-100 p-4 mx-4 mt-2 rounded-lg flex flex-row flex-wrap gap-4">
			<Card url="https://www.andrewteale.me.uk/leap/" name="Local Elections Archive Project (LEAP)" description="Comprehensive Archive of Local Election Results by Andrew Teale"></Card>
			<Card url="http://opencouncildata.co.uk/" name="Open Council Data (OCD)" description="A website with up-to-date collections of council composition data"></Card>
			<Card url="https://www.localcouncils.co.uk/" name="Local Councils" description="Graphical map of UK councils, compositions, boundaries, electoral cycles, etc."></Card>
			<Card url="https://vote-2012.proboards.com/" name="Vote UK Forum" description="Forum containing discussion of local, and national electoral politics in all corners of the UK"></Card>
			<Card url="https://www.britainelects.com/" name="Britain Elects" description="Collection of polling and election results by Ben Walker"></Card>
			<Card url="https://whocanivotefor.co.uk/elections/" name="Democracy Club" description="Collection of all local and national elections in the UK with candidates and polling places."></Card>
			
		</div>
	</div>
</template>
<style scoped>
.text-gradient {
    background-image: linear-gradient(
        -90deg,
        #8DC63F,
        #E4003B,
        #FAA61A,
        #0087DC
    );
    background-size: 400% 400%;
    animation: bg-gradient 10s ease infinite;
}

@keyframes bg-gradient {
    0% {
        background-position: 0% 50%;
    }
    50% {
        background-position: 100% 50%;
    }
    100% {
        background-position: 0% 50%;
    }
}
</style>