<script lang="ts">
  import "../app.postcss";
  import { Drawer, getDrawerStore } from "@skeletonlabs/skeleton";
  import Navigation from "$lib/components/Navigation.svelte";
  import logo from "$lib/assets/logo.png";
  import banner from "$lib/assets/images/thinbanner.png";

  import {
    initializeStores,
  } from "@skeletonlabs/skeleton";

  initializeStores();

  const drawerStore = getDrawerStore();

  function drawerOpen(): void {
    drawerStore.open({});
  }
</script>

<svelte:head>
  <style>
    html, body {
      height: 100%;
      overflow-y: auto;
    }
  </style>
</svelte:head>

<Drawer>
  <Navigation />
</Drawer>

<header class="bg-gradient-to-r from-surface-800 to-primary-900 via-tertiary-900 shadow-2xl">
  <nav class="container mx-auto px-4 py-4">
    <div class="flex items-center justify-between">
      <!-- Mobile menu button -->
      <div class="flex items-center">
        <button class="lg:hidden btn btn-sm mr-4 hover:variant-soft-primary transition-colors" on:click={drawerOpen}>
          <span>
            <svg viewBox="0 0 100 80" class="fill-token w-4 h-4">
              <rect width="100" height="20" />
              <rect y="30" width="100" height="20" />
              <rect y="60" width="100" height="20" />
            </svg>
          </span>
        </button>
        <a href="/" class="flex items-center">
          <img src={logo} alt="Perfect Storm Logo" class="h-12 md:h-28 w-auto" />
        </a>
      </div>

      <!-- Desktop Navigation -->
      <ul class="hidden lg:flex flex-wrap justify-center items-center gap-8 text-2xl md:text-3xl">
        <li><a href="/events" class="hover:text-primary-200 transition-colors">Events</a></li>
        <li><a href="/games" class="hover:text-primary-200 transition-colors">Games</a></li>
        <li><a href="/schedule" class="hover:text-primary-200 transition-colors">Schedule</a></li>
        <li><a href="/venue" class="hover:text-primary-200 transition-colors">Venue</a></li>
        <li><a href="/contact" class="hover:text-primary-200 transition-colors">Contact</a></li>
      </ul>

      <!-- Sign Up Button -->
      <a
        class="btn btn-lg variant-glass text-xl md:text-2xl lg:text-3xl hover:variant-soft-secondary transition-all"
        href="https://www.start.gg/tournament/perfect-storm-2025"
        target="_blank"
        rel="noreferrer"
      >
        Sign Up
      </a>
    </div>
  </nav>
</header>

<div class="flex flex-col min-h-screen">
  <!-- Main Content -->
  <main class="flex-1 container mx-auto px-4 md:px-6 lg:px-8 py-8">
    <slot />
  </main>
</div>
