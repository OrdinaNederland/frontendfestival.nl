<script>
	import HeaderSection from './HeaderSection.svelte';
	import InfoSection from './InfoSection.svelte';
	import PracticalInformationSection from './PracticalInformationSection.svelte';
	import SpeakerScheduleSection from './SpeakerScheduleSection.svelte';
	import SpeakerSection from './SpeakerSection.svelte';
	import WorkshopScheduleSection from './WorkshopScheduleSection.svelte';
</script>

<svelte:head>
	<title>Frontend Festival 2023</title>
	<meta
		name="description"
		content="Let's talk about Frontend: tijdens het Frontend festival nemen we je mee in interessante onderwerpen over Frontend"
	/>
</svelte:head>

<HeaderSection />
<InfoSection />
<SpeakerScheduleSection />
<WorkshopScheduleSection />
<SpeakerSection />
<PracticalInformationSection />
