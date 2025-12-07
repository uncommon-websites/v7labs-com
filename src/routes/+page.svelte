<script lang="ts">
  import Navbar from "$lib/components/Navbar.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import LogoTicker from "$lib/components/LogoTicker.svelte";
  import FeatureSection from "$lib/components/FeatureSection.svelte";
  import LogoGrid from "$lib/components/LogoGrid.svelte";
  import GridFeatures from "$lib/components/GridFeatures.svelte";
  import InteractiveDemo from "$lib/components/InteractiveDemo.svelte";
  import DarkSection from "$lib/components/DarkSection.svelte";
  import VideoGrid from "$lib/components/VideoGrid.svelte";
  import Footer from "$lib/components/Footer.svelte";

  import SpreadsheetVisual from "$lib/components/visuals/SpreadsheetVisual.svelte";
  import IntegrationsVisual from "$lib/components/visuals/IntegrationsVisual.svelte";
  import DocumentsVisual from "$lib/components/visuals/DocumentsVisual.svelte";
  import BrandBookVisual from "$lib/components/visuals/BrandBookVisual.svelte";

  const feature1Tags = [
    { text: "AI Financial Due Diligence Agent", icon: '<span class="w-2 h-2 rounded-full bg-blue-500"></span>' },
    { text: "Legal Risk Identification Agent", icon: '<span class="w-2 h-2 rounded-full bg-purple-500"></span>' },
    { text: "AI LPA Analysis Agent", icon: '<span class="w-2 h-2 rounded-full bg-indigo-500"></span>' },
    { text: "AI Contract Review Agent", icon: '<span class="w-2 h-2 rounded-full bg-orange-500"></span>' },
    { text: "Real Estate Market Analysis Agent", icon: '<span class="w-2 h-2 rounded-full bg-green-500"></span>' },
    { text: "AI Investment Analysis Agent", icon: '<span class="w-2 h-2 rounded-full bg-pink-500"></span>' },
  ];

  const feature2Tags = [
    { text: "Yardi", icon: '<span class="w-3 h-3 bg-blue-600 rounded-sm"></span>' },
    { text: "DealCloud", icon: '<span class="w-3 h-3 bg-blue-800 rounded-sm"></span>' },
    { text: "PitchBook", icon: '<span class="w-3 h-3 bg-black rounded-sm"></span>' },
    { text: "Bloomberg", icon: '<span class="w-3 h-3 bg-black rounded-sm"></span>' },
    { text: "Gmail", icon: '<span class="w-3 h-3 text-red-500 font-bold">M</span>' },
    { text: "Microsoft Outlook", icon: '<span class="w-3 h-3 bg-blue-500 rounded-sm"></span>' },
    { text: "Plain", icon: '<span class="w-3 h-3 bg-black rounded-sm"></span>' },
    { text: "Microsoft Teams", icon: '<span class="w-3 h-3 bg-purple-600 rounded-sm"></span>' },
  ];

  const feature3Tags = [
    { text: "Microsoft SharePoint", icon: '<span class="w-3 h-3 bg-teal-600 rounded-sm"></span>' },
    { text: "Google Drive", icon: '<span class="w-3 h-3 bg-green-600 rounded-sm"></span>' },
    { text: "Snowflake", icon: '<span class="w-3 h-3 bg-blue-400 rounded-sm"></span>' },
    { text: "Databricks", icon: '<span class="w-3 h-3 bg-orange-600 rounded-sm"></span>' },
    { text: "Oracle Cloud Infrastructure", icon: '<span class="w-3 h-3 bg-red-600 rounded-sm"></span>' },
    { text: "Dropbox", icon: '<span class="w-3 h-3 bg-blue-500 rounded-sm"></span>' },
  ];

  const feature4Tags = [
    { text: "Google Slides", icon: '<span class="w-3 h-3 bg-yellow-500 rounded-sm"></span>' },
    { text: "Google Docs", icon: '<span class="w-3 h-3 bg-blue-500 rounded-sm"></span>' },
    { text: "Microsoft PowerPoint", icon: '<span class="w-3 h-3 bg-orange-600 rounded-sm"></span>' },
    { text: "Microsoft Word", icon: '<span class="w-3 h-3 bg-blue-700 rounded-sm"></span>' },
  ];
</script>

<Navbar />

<main>
  <Hero />
  <LogoTicker />
  
  <FeatureSection
    title="Delegate repetitive work"
    subtitle="to the most accurate AI Agents"
    description="Automate document-heavy workflows with unmatched precision—cut manual workload, scale operations, and unlock faster reviews with cleaner outputs and measurable ROI."
    stats={[
      { value: "30%", label: "More accurate than custom GPTs" },
      { value: "n1", label: "On Legalbench and FinanceBench" },
      { value: "20x", label: "ROI on human hours saved by our top customers" }
    ]}
    tags={feature1Tags}
    moreText="+300 more"
    ctaText="Explore agents"
  >
    <SpreadsheetVisual slot="visual" />
  </FeatureSection>

  <FeatureSection
    title="Connect all your apps to AI"
    subtitle="and orchestrate them from one place"
    description="Automate complex workflows across all your tools—seamlessly connecting data, actions, and systems through AI-powered orchestration."
    stats={[
      { value: "400", label: "Supported apps" },
      { value: "6000", label: "Supported actions, already understood by our AI" },
      { value: "100+", label: "Custom integrations supporting your AI product" }
    ]}
    tags={feature2Tags}
    ctaText="Explore integrations"
    reversed={true}
  >
    <IntegrationsVisual slot="visual" />
  </FeatureSection>

  <FeatureSection
    title="All your company's knowledge"
    subtitle="in one place, for humans and AI to use"
    description="Centralize every document, dataset, and insight—giving your teams and AI agents a single source of truth for faster, more accurate decisions."
    stats={[
      { value: "25%", label: "More accurate than RAG" },
      { value: "80", label: "Proprietary indexing data points for deep industry knowledge" },
      { value: "10 million", label: "Data points supported per knowledge hub" }
    ]}
    tags={feature3Tags}
    ctaText="Explore knowledge hubs"
  >
    <DocumentsVisual slot="visual" />
  </FeatureSection>

  <FeatureSection
    title="Generate beautiful documents"
    subtitle="that look as good as 3 hours of work"
    description="Create polished, client-ready documents in seconds—automatically formatted, structured, and tailored to your workflows."
    stats={[
      { value: "25%", label: "More accurate than RAG" },
      { value: "80", label: "Proprietary indexing data points for deep industry knowledge" },
      { value: "10 million", label: "Data points supported per knowledge hub" }
    ]}
    tags={feature4Tags}
    ctaText="Explore document generation"
    reversed={true}
  >
    <BrandBookVisual slot="visual" />
  </FeatureSection>

  <LogoGrid />
  <GridFeatures />
  <InteractiveDemo />
  <DarkSection />
  <VideoGrid />
</main>

<Footer />

