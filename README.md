# CRT-VISUAL-SHADER-GODOT-4.0-

This repository contains a custom CRT (Cathode Ray Tube) shader for the Godot Engine, designed to replicate the nostalgic look of old CRT monitors. The shader includes various effects such as scanlines, screen warping, chromatic aberration, noise, and more, allowing you to create retro-style visuals for your games or projects.

## Features

- **Scanlines**: Simulates the horizontal lines typical of CRT displays.
- **Screen Warping**: Mimics the curvature of old CRT screens.
- **Chromatic Aberration**: Adds a subtle color separation effect.
- **Noise & Static**: Introduces random noise and static for an authentic retro feel.
- **Vignette**: Darkens the edges of the screen for a cinematic effect.
- **Pixelation**: Optionally pixelates the screen for a low-resolution look.
- **Discoloration**: Adds a VHS-style color distortion effect.
- **Roll Effect**: Simulates the rolling effect seen on old CRT TVs.

## Installation

1. Download or clone this repository.
2. Copy the `crt_shader.shader` file into your Godot project's `shaders` directory (or any directory of your choice).
3. Apply the shader to a `CanvasItem` (e.g., a `TextureRect` or `Sprite`) in your scene by selecting the material and assigning the shader.

## Usage

### Uniforms

The shader comes with several customizable uniforms to tweak the CRT effect to your liking:

- **Overlay**: Toggles whether the shader is applied as an overlay.
- **Resolution**: Sets the resolution for pixelation effects.
- **Brightness**: Adjusts the overall brightness of the screen.
- **Scanlines Opacity**: Controls the visibility of scanlines.
- **Scanlines Width**: Adjusts the thickness of scanlines.
- **Grille Opacity**: Controls the opacity of the CRT grille effect.
- **Roll**: Enables or disables the rolling effect.
- **Roll Speed**: Adjusts the speed of the rolling effect.
- **Roll Size**: Controls the size of the rolling effect.
- **Roll Variation**: Adds variation to the rolling effect.
- **Distort Intensity**: Controls the intensity of screen distortion.
- **Aberration**: Adjusts the amount of chromatic aberration.
- **Noise Opacity**: Controls the visibility of noise.
- **Noise Speed**: Adjusts the speed of the noise effect.
- **Static Noise Intensity**: Controls the intensity of static noise.
- **Pixelate**: Toggles pixelation.
- **Discolor**: Toggles VHS-style discoloration.
- **Warp Amount**: Controls the amount of screen warping.
- **Clip Warp**: Clips the warping effect to the screen borders.
- **Vignette Intensity**: Controls the intensity of the vignette effect.
- **Vignette Opacity**: Adjusts the opacity of the vignette.

### Example

```gdscript
# Apply the shader to a TextureRect
var crt_shader = preload("res://shaders/crt_shader.shader")
$TextureRect.material = ShaderMaterial.new()
$TextureRect.material.shader = crt_shader

# Adjust some uniforms
$TextureRect.material.set_shader_param("brightness", 1.2)
$TextureRect.material.set_shader_param("scanlines_opacity", 0.5)
$TextureRect.material.set_shader_param("roll_speed", 10.0)
```

## Contributing

If you have any suggestions, improvements, or bug fixes, feel free to open an issue or submit a pull request. Contributions are always welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments

- Inspired by various CRT shaders and retro-style visual effects.
- Special thanks to the Godot Engine community for their support and resources.

---
