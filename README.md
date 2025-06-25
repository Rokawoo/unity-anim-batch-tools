<div align="center">
  <h1>RΩKΔ's Animation Renamer</h1>
  <p>By RΩKΔ</p>
</div>

> [!CAUTION]
> This scipt makes the impossible... pawssible~! :3

**What is this?**

This is a Unity editor tool that batch renames blend shape properties across multiple animation clips. Made it because I was sick of manually changing blend shape names every time I wanted to transfer animations between different VRChat avatars. You can load a bunch of animation clips, discover all the blend shapes they use, then rename them all at once instead of editing each clip individually. Also handles Japanese characters properly since a lot of good avatars from Booth have Japanese blend shape names.

## How to use:

Drop the script in your `Assets/Editor/` folder or import the unity package, then go to `Tools > RΩKΔ's Animation Renamer` in Unity.

**Basic workflow:**
1. Drag your animation clips into the tool (or entire folders if you're feeling spicy)
2. Hit "Discover Properties" to see all the blend shapes
3. Click on whatever you want to rename to fill the "From" field
4. Type what you want it to be in the "To" field  
5. Hit preview to make sure you're not about to break everything
6. Apply and watch the magic happen

## Common VRChat use cases

**Avatar swapping:** Your old avatar uses "Eye_Blink_L" but your new one uses "BlinkLeft"? Fixed in seconds.

**Booth avatar swapping:** Why do they name their "Head" as "Body"? Change it to it's rightful name! >w<

**Booth asset conversion:** Japanese avatar with "笑顔" that you want to rename to "Smile"? No problem.

**Outfit variants:** Got 5 different outfit versions of the same character? Batch rename all their animations at once.

**MMD imports:** Converting MMD models with their weird naming conventions to something sensible.

The tool is pretty smart about detecting what's a blend shape vs what's just a random animation property, and it won't let you use invalid characters that would break Unity.

## Technical stuff

Built with proper Unicode normalization so Japanese characters don't get mangled. Has validation to prevent you from creating invalid property names. Integrates with Unity's undo system so you can ctrl+z if you mess up. Also has keyboard shortcuts because clicking is for normies.

> [!NOTE]  
> If you find bugs or want features, let me know. This has saved me countless hours and hopefully it'll save you some too :3


<div align="center">
  <h1>RΩKΔ's Animation Property Cleaner</h1>
  <p>By RΩKΔ</p>
</div>

> [!CAUTION]
> This script cleans up your animations like a digital Marie Kondo... if it doesn't spark joy (or have keyframes), it's gone! :3

**What is this?**

This is a Unity editor tool that removes empty and useless properties from animation clips. Made it because I was tired of seeing blend shapes with zero values cluttering up my animations and making the timeline look like a mess. You can load animation clips and it'll find all the properties that are either completely empty (no keyframes) or only have zero/default values, then delete them cleanly. Also handles Japanese characters properly because apparently that's my thing now.

## How to use:

Drop the script in your `Assets/Editor/` folder or import the unity package, then go to `Tools > RΩKΔ's Animation Property Cleaner` in Unity.

**Basic workflow:**
1. Drag your animation clips into the tool (or entire folders because batch operations are life)
2. Choose your cleanup mode (empty properties, zero values, or both)
3. Hit "Discover Empty Properties" to see what's taking up space
4. Hit preview to see exactly what's getting yeeted
5. Apply and watch your animations become clean and minimal

## Common VRChat use cases

**Imported animations:** That MMD animation has 200 blend shapes but only uses 5? Clean it up.

**Recording cleanup:** Recorded an animation but half the blend shapes stayed at 0 the whole time? Gone.

**Avatar optimization:** Remove unused transform properties that got recorded but never actually moved.

**Booth asset cleanup:** Japanese avatars often have tons of unused blend shape channels in their animations.

**Animation merging prep:** Clean up source animations before combining them to avoid conflicts.

The tool has protection options so it won't accidentally delete important stuff like transforms or blend shapes you want to keep, even if they're at zero.

## Technical stuff

Has three cleanup modes: empty properties only, zero-value properties only, or both. Configurable zero threshold so you can decide what counts as "zero enough". Built with the same Japanese character support as the renamer. Full backup system with temporary/permanent options. Integrates with Unity's undo system and has all the same keyboard shortcuts because consistency is key.

> [!NOTE]  
> Pairs perfectly with the Animation Renamer for a complete animation workflow cleanup. Your timeline will thank you :3

