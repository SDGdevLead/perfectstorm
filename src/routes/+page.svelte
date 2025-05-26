<script>
  import tekken from "$lib/assets/games/600px-Tekken-8-logo.png";
  import bbct from "$lib/assets/games/BlazBlue_Cross_Tag_Battle_Logo.png";
  import ggst from "$lib/assets/games/GGStrive_Logo.png";
  import ggxrd from "$lib/assets/games/GGXrdR2_Logo.png";
  import ggxx from "$lib/assets/games/Guilty_Gear_XX_Accent_Core_Plus_R_Logo.png";
  import melee from "$lib/assets/games/Meleelogo.png";
  import p4u from "$lib/assets/games/P4Ulogo.png";
  import scvi from "$lib/assets/games/SCVI Logo.png";
  import sf3 from "$lib/assets/games/SFIII_Online_Edition_Logo.png";
  import sf6 from "$lib/assets/games/Street_Fighter_6_logo.png";
  import uni2 from "$lib/assets/games/UNI2_Logo.png";
  import abkaa from "$lib/assets/games/abkaa.png";
  import bbcf from "$lib/assets/games/bbcf.png";
  import dbfz from "$lib/assets/games/dragonball-fighterz-logo.png";
  import gbvsr from "$lib/assets/games/gbvsr.png";
  import mbaacc from "$lib/assets/games/mbaacc.png";
  import mbtl from "$lib/assets/games/mbtl.png";
  import kof from "$lib/assets/games/top_koflogo.png";
  import umvc from "$lib/assets/games/umvc3.png";
  import vsav from "$lib/assets/games/vsav.png";

  import ttt from "$lib/assets/org/TorontoTopTiers_Logo.png";
  import bc from "$lib/assets/org/battle_city_logo_-_blue_with_white_bg_50.png";
  import dtr from "$lib/assets/org/dtr_logo_rb.png";
  import ecfb from "$lib/assets/org/ecfblogo.png";
  import kizu from "$lib/assets/org/kizuna_transparent.png";

  import banner from "$lib/assets/images/thinbanner.png";
</script>

<div class="space-y-12">
  <div class="text-center space-y-4">
    <p class="gradient-slice text-3xl md:text-4xl lg:text-5xl underline">Marriot Hotel</p>
    <p class="text-xl md:text-2xl lg:text-3xl font-bold">February 12-13, 2025</p>
    <p class="text-xl md:text-2xl lg:text-3xl">100 Kent St, Ottawa Ontario</p>
  </div>

  <div class="container mx-auto px-4 md:px-6 lg:px-8">
    <div class="rounded-container-token drop-shadow-2xl opacity-85 variant-glass-surface text-center p-6 md:p-8 lg:p-12">
      <p class="text-2xl md:text-4xl lg:text-6xl font-bold">Weather the storm in our first organized event!</p>
    </div>
  </div>

  <!-- Games Gallery -->
  <div class="container mx-auto px-4 md:px-6 lg:px-8">
    <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-4 md:gap-6 lg:gap-8">
      {#each [tekken, bbct, ggst, ggxrd, ggxx, melee, p4u, scvi, sf3, sf6, uni2, abkaa, bbcf, dbfz, gbvsr, mbaacc, mbtl, kof, umvc, vsav] as game}
        <div class="group">
          <img
            class="object-contain object-center w-full h-32 md:h-40 lg:h-48 max-w-full rounded-lg drop-shadow-2xl transition-transform duration-300 group-hover:scale-105"
            src={game}
            alt="Game logo"
          />
        </div>
      {/each}
    </div>
  </div>

  <!-- Supporters Section -->
  <div class="container mx-auto px-4 md:px-6 lg:px-8 ">
    <div class="variant-glass-surface opacity-85 rounded-container-token text-center p-6 md:p-8 lg:p-12 mb-8">
      <p class="text-2xl md:text-4xl lg:text-6xl font-bold">Supporters</p>
    </div>
    
    <div class="flex flex-wrap justify-center gap-4 md:gap-6 lg:gap-8">
      {#each [ttt, bc, dtr, ecfb, kizu] as supporter}
        <div class="group w-[45%] sm:w-[30%] md:w-[22%] lg:w-[18%]">
          <img
            class="object-contain object-center w-full h-32 md:h-40 lg:h-48 max-w-full rounded-lg drop-shadow-2xl transition-transform duration-300 group-hover:scale-105"
            src={supporter}
            alt="Supporter logo"
          />
        </div>
      {/each}
    </div>
  </div>
</div>
