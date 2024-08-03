# Kelp to Dried Kelp Block Converter

Litematica schematic: [kelp-to-dried-kelp-block-converter.litematic](./kelp-to-dried-kelp-block-converter.litematic)

Smelts and compresses raw kelp into dried kelp blocks, useful for fueling furnaces.

There are three crafters, labeled with how many slots to fill. The copper bulbs in the schematic are lit and waxed, but lighting and waxing are not necessary. The crafter under the smoker has 0 selected. The middle crafter has 8 selected. The top-most crafter has 1 selected. The smelter needs some bootstrapping fuel to start, but then is self fueling. Needs a constant supply of kelp or will stop working.

Input flows from the top hopper into the smelter. The comparator out of the dried kelp crafter is subtracted from an 8-slot crafter, triggering a bulb which acts as a latch. The latch bulb triggers an observer chain, powering a dropper elevator into a hopper. The hopper refuels the smoker. The top dropper's contents are measured, and once there is a backlog the bottom hopper is unlocked, yielding the profit into the bottom barrel.


![schematic](./ktdkb.png)

---

| ![0 degrees](./ktdkb_000.png) | ![90 degrees](./ktdkb_090.png) |
|:-----------------------------:|:-----------------------------:|
| ![180 degrees](./ktdkb_180.png) | ![270 degrees](./ktdkb_270.png) |
| ![top down](./ktdkb_top.png) |                               |
