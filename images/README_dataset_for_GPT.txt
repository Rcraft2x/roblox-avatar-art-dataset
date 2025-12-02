# Roblox Avatar → Art Dataset
This dataset contains paired examples for converting Roblox avatars into stylized illustrated artwork.  
It is used to guide or train models in transforming raw Roblox avatar images into polished, high-quality art that matches specific visual styles.

---

## 📂 Dataset Structure

### Input Files (Avatar Sources)
Format:
Input_###.png

These images depict raw Roblox avatars.  
They contain no style information and are considered style-neutral.

Examples:
- Input_001.png
- Input_002.png
- …
- Input_020.png

---

### Output Files (Stylized Artwork)
Format:
Output_###_STYLE_ASPECT.png

Where:
- STYLE = the visual art direction  
  (anime, anime_horror, anime_action, oil_painting, sketch, paper_cut, etc.)
- ASPECT = the aspect ratio written using “x”  
  (1x1, 16x9, 9x16, 4x3, etc.)

Examples:
- Output_001_anime_1x1.png  
- Output_013_anime_horror_16x9.png  
- Output_017_oil_painting_1x1.png  
- Output_018_anime_action_16x9.png  

---

## 🔗 Pairing Rule
Every pair is defined by matching the ### number:

Input_###.png  →  Output_###_STYLE_ASPECT.png

Example:
Input_007.png  
Output_007_anime_16x9.png

---

## 🎨 Purpose of the Dataset
The Output images demonstrate how to convert Roblox avatars into stylized illustrated artwork.  
Specifically, they show how to map:

- Roblox proportions → anime or realistic proportions  
- Clothing and accessories → detailed stylized renderings  
- Body colors and shapes → consistent artistic interpretations  
- Hair styles, textures, and colors → illustrated equivalents  
- Expressions and identity → expressive illustrated versions  

They also define how different STYLES behave in terms of:
- lighting  
- shading  
- background density  
- mood and atmosphere  
- line art vs painterly rendering  
- color palette  
- pose and framing  

ASPECT labels define how much of the character is visible and how the scene is composed.

---

## ✔️ STYLE Labels
The dataset includes (so far):

- anime  
- anime_horror  
- anime_action  
- oil_painting  
- paper_cut  
- sketch  

STYLE names must be matched exactly in your GPT or model.

---

## ✔️ ASPECT Labels
Aspect labels in the filename use an “x” for safety:

- 1x1  
- 16x9  
- 9x16  
- 4x3  

When used in prompts or JSON, convert these into:

- 1:1  
- 16:9  
- 9:16  
- 4:3  

---

## 📜 License
This dataset is **private**.  
It may **not** be copied, distributed, or reused without explicit permission from the creator.  
All images and transformations are owned exclusively by the dataset’s creator.