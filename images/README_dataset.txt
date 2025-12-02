Dataset Structure:

Input Files
- Input_###.png
  These are raw Roblox avatar images. They do not contain style or aspect information.

Output Files
- Output_###_STYLE_ASPECT.png
  STYLE = the art style of the final artwork (e.g., anime, neon_noir, soft_pastel)
  ASPECT = the artwork’s aspect ratio written with 'x' instead of ':' (e.g., 1x1, 16x9)

Pairing
- Each Input_### pairs with Output_###_STYLE_ASPECT.
- The GPT uses these pairs to understand:
  • How Roblox models map to illustrated characters
  • How clothing and colors translate to art
  • Style-specific lighting, backgrounds, and proportions
  • Aspect ratio influence on composition

Purpose
This dataset guides the GPT in generating consistent, high-quality illustrated prompts from new Roblox avatar images.