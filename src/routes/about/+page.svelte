<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Intent-driven execution",
			description: "We understand your goals and orchestrate the right tools to achieve them, without the busy work."
		},
		{
			title: "Seamless orchestration", 
			description: "Every system works as one. No more context switching, copy-pasting, or missed connections between tools."
		},
		{
			title: "Human-centered AI",
			description: "Our AI amplifies your decision-making. You focus on strategy while we handle the tool choreography."
		},
		{
			title: "Operational excellence",
			description: "Built by operators who've felt the pain. We know what product teams need because we've been there."
		}
	];
</script>

<SecondaryHero
	generating
	title="Solving world hunger"
	subtitle="one step at a time"
	imageSrc="https://www.unc.mn/image-placeholder.svg"
/>

<!-- Story Section -->
<Story
	generating
	paragraphs={[
		"We started in 2018 with a simple goal: make helpful tech that people actually need. While many chase profits, we chose to do things differently.",
		"Beyond making good products, we care about doing the right thing, being kind to our planet, and making sure everyone can use what we build. That's our compass.",
		"From day one, we've asked ourselves: 'Does this actually help people?' This question gets us through tough calls and shapes who we are. We're playing the long game here.",
		"We think about how our work affects real people's lives. We build tech that brings people together, keeps your information safe, and treats everyone fairly. When we stick to these basics, good things happen."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our team."
	subtitle="Connecting AI models with unified tool orchestration."
	stakeholders={[
		{
			name: "Rajiv Sancheti",
			position: "Founder",
			bio: "Visionary founder focused on eliminating tool-switching overhead for knowledge workers.",
			image: "/generated/image-professional-headshot-business-portrait-.webp"
		},
		{
			name: "Connor Waslo",
			position: "Founder",
			bio: "Co-founder dedicated to building the first true intent-based interface for workplace automation.",
			image: "/generated/image-professional-headshot-business-portrait-.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Stop losing hours to tool switching"
	subtitle="Get early access"
	description="Product managers at fast-growing companies are saving 3+ hours daily by orchestrating all their tools through one intent-driven interface. See how much faster your team can move when everything just clicks together."
	imageSrc="/generated/image-a-professional-product-manager-confident.webp"
/>
