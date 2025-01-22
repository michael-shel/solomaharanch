<script>
  const links = [
    {
      name: "Google Drive",
      url: "https://drive.google.com/file/d/1lqAmWXge-b0HmnPcJ1-E4cg2gbEbbvm7/view",
      icon: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M12 2L2 7v10l10 5 10-5V7l-10-5zm0 13l-5-3-5 3V8l5-3 5 3v7z" fill="#4285F4"/></svg>`,
      label: "Access the document on Google Drive",
    },
    {
      name: "Instagram (EquiRehab Ukraine)",
      url: "https://www.instagram.com/equirehab.ukraine/",
      icon: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M12 2c1.65 0 3.17.63 4.29 1.75C17.37 4.83 18 6.35 18 8s-.63 3.17-1.71 4.25C15.17 13.37 13.65 14 12 14s-3.17-.63-4.29-1.75C6.63 10.83 6 9.35 6 8s.63-3.17 1.71-4.25C8.83 2.63 10.35 2 12 2zm0 3c-.98 0-1.9.37-2.58.97-.68.6-1.02 1.43-1.02 2.3s.34 1.7 1.02 2.3C10.1 8.63 11.02 9 12 9s1.9-.37 2.58-.97c.68-.6 1.02-1.43 1.02-2.3s-.34-1.7-1.02-2.3C13.9 5.37 12.98 5 12 5zm6.5 2.5c-.22 0-.44.08-.62.24-.18.18-.26.4-.26.62s.08.44.26.62c.18.18.4.26.62.26s.44-.08.62-.26c.18-.18.26-.4.26-.62s-.08-.44-.26-.62c-.18-.16-.4-.24-.62-.24z" fill="#E4405F"/></svg>`,
      label: "Visit EquiRehab Ukraine on Instagram",
    },
    {
      name: "Facebook (Solomaha Ranch)",
      url: "https://www.facebook.com/solomaha.ranch/",
      icon: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M22.7 0H1.3C.6 0 0 .6 0 1.3v21.4c0 .7.6 1.3 1.3 1.3h11.9v-9.3h-3v-3.6h3v-2.7c0-4.2 2.4-6.4 6.2-6.4 1.8 0 3.6.1 4.1.2v3.5h-2.8c-2.2 0-2.7 1-2.7 2.5v3.3h5.4l-1.1 3.6h-4.3v9.3h8.5c.7 0 1.3-.6 1.3-1.3V1.3c0-.7-.6-1.3-1.3-1.3z" fill="#1877F2"/></svg>`,
      label: "Visit Solomaha Ranch on Facebook",
    },
    {
      name: "Instagram (Solomaha Ranch)",
      url: "https://www.instagram.com/solomaharanch/",
      icon: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M12 2c1.65 0 3.17.63 4.29 1.75C17.37 4.83 18 6.35 18 8s-.63 3.17-1.71 4.25C15.17 13.37 13.65 14 12 14s-3.17-.63-4.29-1.75C6.63 10.83 6 9.35 6 8s.63-3.17 1.71-4.25C8.83 2.63 10.35 2 12 2zm0 3c-.98 0-1.9.37-2.58.97-.68.6-1.02 1.43-1.02 2.3s.34 1.7 1.02 2.3C10.1 8.63 11.02 9 12 9s1.9-.37 2.58-.97c.68-.6 1.02-1.43 1.02-2.3s-.34-1.7-1.02-2.3C13.9 5.37 12.98 5 12 5zm6.5 2.5c-.22 0-.44.08-.62.24-.18.18-.26.4-.26.62s.08.44.26.62c.18.18.4.26.62.26s.44-.08.62-.26c.18-.18.26-.4.26-.62s-.08-.44-.26-.62c-.18-.16-.4-.24-.62-.24z" fill="#E4405F"/></svg>`,
      label: "Visit Solomaha Ranch on Instagram",
    },
    {
      name: "Facebook (EquiRehab Ukraine)",
      url: "https://www.facebook.com/equirehab.ukraine/",
      icon: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M22.7 0H1.3C.6 0 0 .6 0 1.3v21.4c0 .7.6 1.3 1.3 1.3h11.9v-9.3h-3v-3.6h3v-2.7c0-4.2 2.4-6.4 6.2-6.4 1.8 0 3.6.1 4.1.2v3.5h-2.8c-2.2 0-2.7 1-2.7 2.5v3.3h5.4l-1.1 3.6h-4.3v9.3h8.5c.7 0 1.3-.6 1.3-1.3V1.3c0-.7-.6-1.3-1.3-1.3z" fill="#1877F2"/></svg>`,
      label: "Visit EquiRehab Ukraine on Facebook",
    },
  ];
</script>

<style>
  .link-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1rem;
    margin: 2rem auto;
    width: 100%;
    max-width: 600px;
  }

  .link-item {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    background: #f9f9f9;
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 0.75rem 1rem;
    width: 100%;
    text-decoration: none;
    color: #333;
    font-size: 1rem;
    transition: background-color 0.3s ease, transform 0.2s ease;
  }

  .link-item:hover {
    background-color: #e6f7ff;
    transform: scale(1.03);
  }

  .link-item svg {
    height: 24px;
    width: 24px;
  }

  .link-item span {
    flex: 1;
    text-align: left;
  }

  @media (max-width: 480px) {
    .link-item {
      font-size: 0.875rem;
      padding: 0.5rem;
    }

    .link-item svg {
      height: 20px;
      width: 20px;
    }
  }
</style>

<div class="link-container">
  {#each links as { name, url, icon, label }}
    <a
      class="link-item"
      href="{url}"
      target="_blank"
      rel="noopener noreferrer"
      aria-label="{label}"
    >
      <span>{name}</span>
    </a>
  {/each}
</div>
