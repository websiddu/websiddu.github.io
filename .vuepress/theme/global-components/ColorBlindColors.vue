<template>
  <div class="palettes">
    <div class="palette" v-for="(hue, i) in hues" :key="i">
      <div class="clr" v-for="(clr, j) in hue" :key="j">
        <div class="clr-block" :style="{background: clr}"></div>
        {{clr}}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      hues: [
        [
          "#f7fcfd",
          "#e5f5f9",
          "#ccece6",
          "#99d8c9",
          "#66c2a4",
          "#41ae76",
          "#238b45",
          "#006d2c",
          "#00441b"
        ],
        [
          "#f7fcfd",
          "#e0ecf4",
          "#bfd3e6",
          "#9ebcda",
          "#8c96c6",
          "#8c6bb1",
          "#88419d",
          "#810f7c",
          "#4d004b"
        ],
        [
          "#f7fcf0",
          "#e0f3db",
          "#ccebc5",
          "#a8ddb5",
          "#7bccc4",
          "#4eb3d3",
          "#2b8cbe",
          "#0868ac",
          "#084081"
        ],
        [
          "#fff7ec",
          "#fee8c8",
          "#fdd49e",
          "#fdbb84",
          "#fc8d59",
          "#ef6548",
          "#d7301f",
          "#b30000",
          "#7f0000"
        ],
        [
          "#fff7fb",
          "#ece7f2",
          "#d0d1e6",
          "#a6bddb",
          "#74a9cf",
          "#3690c0",
          "#0570b0",
          "#045a8d",
          "#023858"
        ],
        [
          "#fff7fb",
          "#ece2f0",
          "#d0d1e6",
          "#a6bddb",
          "#67a9cf",
          "#3690c0",
          "#02818a",
          "#016c59",
          "#014636"
        ],
        [
          "#f7f4f9",
          "#e7e1ef",
          "#d4b9da",
          "#c994c7",
          "#df65b0",
          "#e7298a",
          "#ce1256",
          "#980043",
          "#67001f"
        ],
        [
          "#fff7f3",
          "#fde0dd",
          "#fcc5c0",
          "#fa9fb5",
          "#f768a1",
          "#dd3497",
          "#ae017e",
          "#7a0177",
          "#49006a"
        ],
        [
          "#ffffe5",
          "#f7fcb9",
          "#d9f0a3",
          "#addd8e",
          "#78c679",
          "#41ab5d",
          "#238443",
          "#006837",
          "#004529"
        ],
        [
          "#ffffd9",
          "#edf8b1",
          "#c7e9b4",
          "#7fcdbb",
          "#41b6c4",
          "#1d91c0",
          "#225ea8",
          "#253494",
          "#081d58"
        ],
        [
          "#ffffe5",
          "#fff7bc",
          "#fee391",
          "#fec44f",
          "#fe9929",
          "#ec7014",
          "#cc4c02",
          "#993404",
          "#662506"
        ],
        [
          "#ffffcc",
          "#ffeda0",
          "#fed976",
          "#feb24c",
          "#fd8d3c",
          "#fc4e2a",
          "#e31a1c",
          "#bd0026",
          "#800026"
        ],
        [
          "#f7fbff",
          "#deebf7",
          "#c6dbef",
          "#9ecae1",
          "#6baed6",
          "#4292c6",
          "#2171b5",
          "#08519c",
          "#08306b"
        ],
        [
          "#ffffff",
          "#f0f0f0",
          "#d9d9d9",
          "#bdbdbd",
          "#969696",
          "#737373",
          "#525252",
          "#252525",
          "#000000"
        ],
        [
          "#f7fcf5",
          "#e5f5e0",
          "#c7e9c0",
          "#a1d99b",
          "#74c476",
          "#41ab5d",
          "#238b45",
          "#006d2c",
          "#00441b"
        ],
        [
          "#fcfbfd",
          "#efedf5",
          "#dadaeb",
          "#bcbddc",
          "#9e9ac8",
          "#807dba",
          "#6a51a3",
          "#54278f",
          "#3f007d"
        ],
        [
          "#fff5f0",
          "#fee0d2",
          "#fcbba1",
          "#fc9272",
          "#fb6a4a",
          "#ef3b2c",
          "#cb181d",
          "#a50f15",
          "#67000d"
        ],
        [
          "#fff5eb",
          "#fee6ce",
          "#fdd0a2",
          "#fdae6b",
          "#fd8d3c",
          "#f16913",
          "#d94801",
          "#a63603",
          "#7f2704"
        ]
      ]
    };
  }
};
</script>

<style lang="stylus">
.palettes {
  display: flex;
  flex-wrap: wrap;

  .palette {
    flex: 1;
    margin-right: 24px;
    margin-bottom: 24px;
  }

  .clr {
    height: 32px;
    display: flex;
    align-items: center;
    font-size: 12px;
    font-weight: 500;
    text-transform: uppercase;
    color: #5f6368;

    .clr-block {
      height: 32px;
      width: 30px;
      margin-right: 8px;
    }
  }
}
</style>
