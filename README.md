<img src="https://github.com/user-attachments/assets/8f0a9839-7b83-476b-be41-ac1f449356d4" alt="The Better Roles Logo" width="800" height="300">

## Cosmetics Creation Guide

## Hat Creation  

A hat consists of multiple textures. The recommended texture resolution is **300px x 375px** with a **4:5 aspect ratio**.  

### Required Textures  
1. **Main Texture** (`sprite`):  
   - The primary texture of your hat.  
   - Rendered in front of the player.
   - File name pattern: `hatname.png`.  
   - Optional Parameters in the configuration:  
     - `bounce`: Makes the hat bounce when the player moves.  
     - `colorbase`: Uses the player's color shader (e.g., red (#ff0000) is replaced with the player's primary color, blue (#0000ff) with the secondary color).  
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

## Hat Configuration
```json
{
  "package": "The Better Hats", // Category displayed in cosmetics menu
  "id": "hat_template", // Unique ID (lowercase, no spaces)
  "name": "Hat Template", // Display name in game
  "author": "Author Name", // Creator credit
  "folder": "HatTemplate_Folder", // Must match folder name
  "sprite": "template_hat.png", // Main front texture (required)
  "flipsprite": "template_hat_flip.png", // Left-facing version (optional)
  "backsprite": "template_hat_back.png", // Back texture (optional)
  "flipbacksprite": "template_hat_flipback.png", // Left-facing back texture (optional)
  "climbsprite": "template_hat_climb.png", // Ladder climbing texture (required)
  "behind": false, // true = renders behind player
  "bounce": true, // true = adds bounce animation when moving
  "colorbase": false // true = uses player's color palette
}
```
---

## Visor Creation  

Visors require fewer textures than hats. Recommended resolution is **300px x 375px** with a **4:5 aspect ratio**.

### Required Textures
1. **Main Texture** (`sprite`):
   - Primary visor texture
   - File name pattern: `visorname.png`
   
2. **Climbing Texture** (`climbsprite`):
   - Used when climbing ladders
   - File name pattern: `visorname_climb.png`

### Optional Textures
1. **Flipped Texture** (`flipsprite`):
   - Used when player faces left
   - File name pattern: `visorname_flip.png`

## Visor Configuration
```json
{
  "package": "The Better Visors", // Category displayed in cosmetics menu
  "id": "visor_template", // Unique ID (lowercase, no spaces)
  "name": "Visor Template", // Display name in game
  "author": "Author Name", // Creator credit
  "folder": "VisorTemplate_Folder", // Must match folder name
  "sprite": "template_visor.png", // Main texture (required)
  "flipsprite": "template_visor_flip.png", // Left-facing version (optional)
  "climbsprite": "template_visor_climb.png", // Ladder climbing texture (required)
  "behindhats": false, // true = renders behind hats
  "colorbase": false // true = uses player's color palette
}
```
---

## Skin Creation  

Skins require special attention to spritesheets. Use existing game skins as reference.

### Required Textures
1. **Spritesheet** (`sprite`):
   - Must match an existing game skin's format
   - File name pattern: `skinname_spritesheet.png`
   
2. **Preview Image** (`preview`):
   - Displayed in cosmetics menu
   - File name pattern: `skinname_preview.png`

## Skin Configuration
```json
{
  "package": "The Better Skins", // Category displayed in cosmetics menu
  "id": "skin_template", // Unique ID (lowercase, no spaces)
  "name": "Skin Template", // Display name in game
  "author": "Author Name", // Creator credit
  "folder": "SkinTemplate_Folder", // Must match folder name
  "sprite": "template_skin_spritesheet.png", // Animation spritesheet (required)
  "preview": "template_skin_preview.png", // Menu preview image (required)
  "ref_skin_id": "skin_SuitB", // Original skin ID being replaced (required)
  "colorbase": false // true = uses player's color palette
}
```
---

## Nameplate Creation  

Nameplates are the simplest cosmetic with just one required texture. Recommended resolution is **275px x 66px** with a **25:6 aspect ratio**.

### Required Texture
1. **Main Texture** (`sprite`):
   - Displayed on player nameplate in meetings.
   - File name pattern: `nameplatename.png`

## Nameplate Configuration
```json
{
  "package": "The Better Nameplates", // Category displayed in cosmetics menu
  "id": "nameplatetemplate", // Unique ID (lowercase, no spaces)
  "name": "Name Plate Template", // Display name in game
  "author": "Author Name", // Creator credit
  "folder": "NamePlateTemplate_Folder", // Must match folder name
  "sprite": "template_nameplate.png" // Texture file (required)
}
```
---

## Template  
We've created template files for all cosmetics here: [Template Folder](https://github.com/D1GQ/TBR_Hats/tree/main/Template)

---

## Testing Your Cosmetics  
- Place new cosmetic folders in their respective directories under:
  - `Among Us/BetterRole_Data/Cosmetics/[Hats|Visors|Skins|Nameplates]`
- Note that these folders might be hidden - enable "show hidden files" in your OS settings.

---

## Submission Guidelines  
- **Original Content Only:** Do not submit content from other mods or containing licensed material.  
- **How to Submit:**  
  - Share your designs on our [Discord](https://discord.com/invite/ten).  
  - Submit either screenshots or the files directly.  

We can't wait to see your amazing designs! 🎨  
