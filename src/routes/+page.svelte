<script>
  import { Section, News, HeroHeader, HeroBody } from 'flowbite-svelte-blocks';
 
</script>

<Section name="heroDefault">
  <News>
    <span class="text-xs bg-primary-600 rounded-full text-white px-4 py-1.5 mr-3">New</span>
    <span class="text-sm font-medium">Flowbite is out! See what's new</span>
  </News>
  <HeroHeader>
    <svelte:fragment slot="h1">We invest in the world’s potential</svelte:fragment>
    <svelte:fragment slot="paragraph">Here at Flowbite we focus on markets where technology, innovation, and capital can unlock long-term value and drive economic growth.</svelte:fragment>
  </HeroHeader>
</Section>