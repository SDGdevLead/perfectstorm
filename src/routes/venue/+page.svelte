<script lang="ts">
  import marriot from "$lib/assets/venue/marriot.jpg";
  import room from "$lib/assets/venue/room.png";
  import walk from "$lib/assets/venue/walk.png";
</script>

<div class="flex flex-wrap justify-center py-10">
  <p class="px-4 text-3xl md:text-4xl lg:text-6xl font-bold text-center">
    PerfectStorm will be held at the Marriot Hotel meeting facility
  </p>
</div>

<div class="flex flex-wrap justify-start gap-4 p-12">
  <img class="rounded-container-token" src={marriot} alt="marriotImage" />
  <img class="rounded-container-token" src={room} alt="roomImage" />
</div>

<div class="flex flex-wrap justify-center py-10">
  <p class="px-4 text-3xl md:text-4xl lg:text-6xl font-bold text-center">
    Which is easily accessible from the Lyon LRT station
  </p>
</div>

<div class="flex flex-wrap justify-center gap-4 p-10">
  <img class="rounded-container-token" src={walk} alt="walkImage" />
</div>
