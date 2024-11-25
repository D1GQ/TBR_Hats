<img src="https://github.com/user-attachments/assets/8f0a9839-7b83-476b-be41-ac1f449356d4" alt="The Better Roles Logo" width="800" height="300">

## Hat Creation  

A hat consists of multiple textures. The recommended texture resolution is **300px x 375px** with a **4:5 aspect ratio**.  

### Required Textures  
1. **Main Texture** (`sprite`):  
   - The primary texture of your hat.  
   - Rendered in front of the player.
   - File name pattern: `hatname.png`.  
   - Optional Parameters in the configuration:  
     - `bounce`: Makes the hat bounce when the player moves.  
     - `colorbase`: Uses the player’s color shader (e.g., red (#ff0000) is replaced with the player’s primary color, blue (#0000ff) with the secondary color).  
     - `behind`: Renders the hat behind the player.  

2. **Climbing Texture** (`climbsprite`):  
   - Used when the player climbs a ladder.  
   - File name pattern: `hatname_climb.png`.  

---

### Optional Textures  
1. **Back Texture** (`backsprite`):  
   - Renders behind the player.  
   - File name pattern: `hatname_back.png`.  

2. **Flipped Texture** (`flipsprite`):  
   - Used when the player faces left.  
   - File name pattern: `hatname_flip.png`.  

3. **Flipped Back Texture** (`flipbacksprite`):  
   - Back texture for when the player faces left.  
   - File name pattern: `hatname_flipback.png`.  

---

## Template  
We’ve created a template file with the config here [Template](https://github.com/D1GQ/TBR_Hats/tree/main/Template/HatTemplate_Folder)

---

## Testing Your Hat  
- Place the new hat folder in the `Among Us/BetterRole_Data/Hats` folder.
- Note that the `Hats` folder is hidden so be sure to have show hidden files enabled!

---

## Submission Guidelines  
- **Original Content Only:** Please do not submit hats from other mods or designs containing licensed materials.  
- **How to Submit:**  
  - Share your design on our Discord.  
  - You can submit either screenshots of your hat in action or the hat files directly.  

We can't wait to see your amazing designs! 🎨  
