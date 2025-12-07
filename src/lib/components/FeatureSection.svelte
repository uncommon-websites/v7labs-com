<script lang="ts">
  export let title: string;
  export let subtitle: string = "";
  export let description: string;
  export let stats: { value: string; label: string }[] = [];
  export let tags: { text: string; icon?: any }[] = [];
  export let moreText: string = "+400 more";
  export let ctaText: string = "Explore agents";
  export let reversed: boolean = false;
  export let bgColor: string = "bg-white";
</script>

<section class="{bgColor} py-24 px-6 overflow-hidden">
  <div class="max-w-7xl mx-auto">
    <div class="flex flex-col lg:flex-row gap-16 lg:gap-24 {reversed ? 'lg:flex-row-reverse' : ''}">
      
      <!-- Content Side -->
      <div class="flex-1 flex flex-col justify-center">
        <h2 class="text-3xl md:text-4xl font-medium text-gray-900 mb-2 tracking-tight">
          {title}
        </h2>
        {#if subtitle}
          <p class="text-3xl md:text-4xl font-medium text-gray-400 mb-6 tracking-tight">
            {subtitle}
          </p>
        {/if}
        
        <p class="text-lg text-gray-600 mb-8 leading-relaxed max-w-lg">
          {description}
        </p>

        {#if tags.length > 0}
          <div class="mb-4 text-xs font-medium text-gray-400 uppercase tracking-wider">
            {#if title.includes("Delegate")}
              Get started automating
            {:else if title.includes("Connect")}
              Including professional SaaS like
            {:else if title.includes("knowledge")}
              Connect all your data from
            {:else if title.includes("beautiful")}
              Compatible with
            {/if}
          </div>
          <div class="flex flex-wrap gap-2 mb-8">
            {#each tags as tag}
              <div class="inline-flex items-center gap-1.5 px-3 py-1.5 rounded-full border border-gray-200 bg-white text-xs font-medium text-gray-700 hover:border-gray-300 transition-colors cursor-default">
                {#if tag.icon}
                  {@html tag.icon}
                {/if}
                {tag.text}
              </div>
            {/each}
            <div class="inline-flex items-center px-3 py-1.5 text-xs text-gray-400">
              {moreText}
            </div>
          </div>
        {/if}

        <a href="#" class="inline-flex items-center text-sm font-medium text-gray-900 hover:underline decoration-1 underline-offset-4 mb-12">
          {ctaText}
          <svg class="ml-1 w-4 h-4 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
        </a>

        <!-- Stats -->
        {#if stats.length > 0}
          <div class="grid grid-cols-3 gap-8 border-t border-gray-100 pt-8">
            {#each stats as stat}
              <div>
                <div class="text-3xl font-medium text-gray-900 mb-1">{stat.value}</div>
                <div class="text-xs text-gray-500 leading-snug">{stat.label}</div>
              </div>
            {/each}
          </div>
        {/if}
      </div>

      <!-- Visual Side -->
      <div class="flex-1 relative min-h-[400px] bg-gray-50 rounded-2xl overflow-hidden">
        <slot name="visual" />
      </div>

    </div>
  </div>
</section>
