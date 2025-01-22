<script lang="ts">
  import { page } from "$app/stores";

  const links = [
    {
      name: "Буклет програми реабілітації",
      href: "https://drive.google.com/file/d/1lqAmWXge-b0HmnPcJ1-E4cg2gbEbbvm7/view",
      icon: "./brochure.png",
    },
    {
      name: "Facebook EquiRehab",
      href: "https://www.facebook.com/equirehab.ukraine/",
      icon: "./facebook.png",
    },
    {
      name: "Instagram EquiRehab",
      href: "https://www.instagram.com/equirehab.ukraine/",
      icon: "./instagram.webp",
    },
    {
      name: "Facebook Solomaha Ranch",
      href: "https://www.facebook.com/solomaha.ranch/",
      icon: "./facebook.png",
    },
    {
      name: "Instagram Solomaha Ranch",
      href: "https://www.instagram.com/solomaharanch/",
      icon: "./instagram.webp",
    },
  ];

  console.log("page", $page);
</script>

<svelte:head>
  <title>EquiRehab</title>
  <link rel="icon" href="{$page.url.origin}/logo.png" />
  <meta property="image" content="{$page.url.origin}/logo.png" />
  <meta name="description" content="EquiRehab LinksTree" />
  <meta property="og_site_name" content="EquiRehab LinksTree" />
  <meta
    property="og:url"
    content="https://www.instagram.com/equirehab.ukraine"
  />
  <meta property="og:type" content="website" />
  <meta property="og:title" content="EquiRehab" />
  <meta property="og:description" content="EquiRehab SolomahaRanch LinksTree" />
  <meta property="og:image" content="{$page.url.origin}/logo.png" />
  <meta name="twitter:title" content="EquiRehab" />
  <meta
    name="twitter:description"
    content="EquiRehab SolomahaRanch LinksTree"
  />
  <meta name="twitter:image" content="{$page.url.origin}/logo.png" />
  <meta name="twitter:card" content="summary_large_image" />
</svelte:head>

<div
  class="flex bg-white min-h-screen flex-col justify-center gap-10 pt-10 items-center"
>
  <div class="flex w-full justify-center items-center px-5 max-w-52">
    <img src="./logo.png" alt="Logo" />
  </div>

  <div
    class="flex justify-start gap-5 flex-col items-center flex-1 md:flex-none"
  >
    {#each links as { name, href, icon }}
      <div
        class="flex gap-2.5 items-center rounded-lg bg-mint shadow-sm shadow-brown p-2.5 w-full md:min-w-96 hover:bg-brown transition-all"
      >
        <img class="w-5 h-5" src={icon} alt={name} />
        <a class="text-white text-lg font-medium" {href}
          >{name}</a
        >
      </div>
    {/each}
  </div>
</div>
