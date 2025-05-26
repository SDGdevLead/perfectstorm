<script lang="ts">
  import marriot from "$lib/assets/venue/marriot.jpg";
  import room from "$lib/assets/venue/room.png";
  import walk from "$lib/assets/venue/walk.png";
</script>

<div class="container mx-auto px-4 py-16">
  <h1 class="text-2xl md:text-3xl lg:text-4xl font-bold text-center mb-16">
    PerfectStorm will be held at the Marriot Hotel meeting facility
  </h1>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-16">
    <div class="flex justify-center">
      <img 
        class="rounded-lg shadow-lg w-full max-w-2xl object-cover" 
        src={marriot} 
        alt="Marriot Hotel exterior" 
      />
    </div>
    <div class="flex justify-center">
      <img 
        class="rounded-lg shadow-lg w-full max-w-2xl object-cover" 
        src={room} 
        alt="Meeting room interior" 
      />
    </div>
  </div>

  <h2 class="text-3xl md:text-4xl lg:text-6xl font-bold text-center mb-16">
    Which is easily accessible from the Lyon LRT station
  </h2>

  <div class="flex justify-center mb-16">
    <img 
      class="rounded-lg shadow-lg w-full max-w-4xl object-cover" 
      src={walk} 
      alt="Walking route from LRT station" 
    />
  </div>
</div>
