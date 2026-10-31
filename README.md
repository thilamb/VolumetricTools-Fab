# VolumetricTools-Fab

This is a FREE Unreal Engine plugin, available on Fab, that adds Volume assets features in the editor.

The plugin can:
* Convert **Static Vector Field assets** into **Volume Texture assets**, preserving dimensions and voxel data.
* Convert **Sparse Volume Texture assets** into (dense) **Volume Texture assets**, with same size or with downsizing.
* Apply any **mathematical operation on texture values**, creating a new Texture or modifying source texture in-place.

## Table of Contents
- [Install](#Install)
- [Vector Field to Volume Textures](#Vector-Field-To-Volume-Texture)
- [SVT to Volume Texture](#Sparse-Volume-Texture-(SVT)-to-Volume-Texture)
- [Math Expression on Textures](#Modify-Texture-values)


## Install

First make sure that the plugin is enabled:
<img width="1058" height="267" alt="image" src="https://github.com/user-attachments/assets/cf446b82-0347-490e-bb64-a172ec2db18f" />

## Vector Field To Volume Texture

Right click on any vector static field, and select **Convert to Volume Texture**. 
<img width="1062" height="326" alt="2026-10-31 15_53_21-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/71798fa3-1d64-46c4-ae68-6881c9e9b049" />

A new Volume Texture will be created in the same folder.
<img width="1447" height="968" alt="DisplayVolume" src="https://github.com/user-attachments/assets/c6fda7e0-9c99-4a25-ba4f-0e082d388d90" />


## Sparse Volume Texture (SVT) to Volume Texture

Right click on any Sparse Volume Texture, select **Convert to Dense Volume Texture**.

You'll have the option to choose from Attribute A or B, to convert just the first channel (R) or first three (RGB) or all channels.

You can keep the original size, or downsize to some cubic sizes. When downsizing, you will loose the original volume ratio.

## Modify Texture values

Right click on any Texture (2D or Volume) to change its values, select **Apply Math Expression**. You'll be able to apply math expressions to all values of the texture. The operation can create a new texture or directly change values on the same texture.

Allowed math operations are: `+, -, *, /, ^, (, ), abs, floor, ceil, sqrt, log, exp, pow, min, max, clamp`.

1. <img width="964" height="288" alt="2026-10-31 15_28_09-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/06078e06-46c5-4656-b8f5-5ecdc392129d" />

2. <img width="489" height="258" alt="2026-10-31 15_31_04-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/91376b3a-4c88-45ba-a6f2-57cfee56b8f0" />

3. <img width="232" height="188" alt="2026-10-31 15_31_23-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/f77e3f77-e7c0-49b8-9fa6-54da53e433cb" />

4. Also works on Volume Textures:
<img width="627" height="297" alt="2026-10-31 15_37_16-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/3b85683c-c5d8-428e-b7c2-ed2a706ee851" />


Enjoy.
