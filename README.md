# mv-shaders

> Some shaders for [MagicaVoxel](https://ephtracy.github.io/) to make some tedious tasks easier.

## Installation

[Download the latest release](https://github.com/knosvoxel/mv-shaders/releases/) and copy the files from the `shader` directory of your MagicaVoxel installation.

## Shaders

### Grass

The grass shader currently comes in 4 different variations:

- **grass**: Voxels are placed on all surfaces at random based on your selected `color index` in the palette. You can choose a `seed` and `threshold`. A higher threshold means that less voxels will be placed.
- **grass_color**: Works very similar to the `grass` shader. The main difference is that you can decide what color index should be used by adjusting the `Color` parameter. Voxels will only be placed on voxels that are the same color value as the one you have selected in your palette. Adjusting the `Color Threshold` can be used to adjust how much of your selected color and the color parameter is used, giving it a bit of randomness between the two.
- **grass_offset**: After making basic grass blades with the `grass` shader you can use this shader to add some bend to them. Based on the color you select in the palette you can decide which index is affected. Voxels are placed on top and offset by 1 in the direction you determine by adjusting the `Mode`. There are 8 different modes for all basic directions.
- **grass_offset_color**: Similar to the `grass_color` shader this shader gives you more control over the color of voxels that are placed. It also comes with a similar threshold level to adjust the blend between the 2 colors that are used.

### Snow

The snow shader currently comes in 2 different variations:

- **snow**: This shader has two `modes`:
  - Mode 1: Voxels that don't have a voxel on layer above them are replaced with the color you have selected in the palette
  - Mode 2: Only voxels that don't have a voxel above them at all are replaced.
- **snow_add**: This shader also has two `modes`with similar differences as the `snow` shader. The only difference is that in this case voxels aren't replaced but voxels are added one layer above those voxels already present with the color you have selected in your palette.

### Sand

The sand shader currently only has one variation:

- **sand_brush**: This shader takes voxels with the selected color index's color and makes them "fall down" one voxel with each usage of the shader

## Feedback & Ideas

If there is any feedback you have or ideas for new shaders head over to the Issues tab and and [create a new issue][new-issue] if one doesn't exist already for the same thing or send me a message on Discord `knosvoxel#4773`

## License

This repository is licenced under the [MIT license][license-link].

[new-issue]: https://github.com/knosvoxel/mv-shaders/issues/new
[license-link]: https://github.com/knosvoxel/mv-shaders/blob/main/LICENSE
