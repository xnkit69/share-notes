<script>
  import '../app.postcss';

  import { Icon } from '@steeze-ui/svelte-icon';
  import { Github } from '@steeze-ui/lucide-icons';
</script>

<svelte:head>
  <meta name="keywords" content="Share Notes, e2e, note, sharing, end-to-end, encrypted, open source, free" />
  <meta property="language" content="en" />
</svelte:head>

<div class="contain">
  <div class="flex justify-between items-center mb-4">
    <a href="/">
      <h1 class="text-2xl font-black">Share Notes</h1>
      <span class="text-xs text-neutral-800 dark:text-neutral-400">- e2e note sharing</span>
    </a>
    <div class="flex gap-2 items-center">
      <a
        href="https://github.com/xnkit69"
        class="p-2 rounded-full dark:hover:bg-neutral-900 hover:bg-neutral-100"
      >
        <Icon src={Github} class="w-6 h-6" />
        <span class="sr-only">GtHub</span>
      </a>
    </div>
  </div>
  <slot />
</div>
