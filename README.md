# VolumetricTools-Fab

This is a FREE Unreal Engine plugin, available on Fab. It is a collection of editor utilities for manipulating volume textures and streamlining volumetric workflows.

The plugin can:
* Convert **Static Vector Field assets** into **Volume Texture assets**, preserving dimensions and voxel data.
* Convert **Sparse Volume Texture assets** into (dense) **Volume Texture assets**, with options to preserve the original resolution or downsample to a smaller size.
* Apply **mathematical operations to texture values**, either creating a new texture or modifying the source texture in place.

## Table of Contents
- [Install](#Install)
- [Vector Field to Volume Textures](#Vector-Field-To-Volume-Texture)
- [SVT to Volume Texture](#Sparse-Volume-Texture-to-Volume-Texture)
- [Math Expression on Textures](#Modify-Texture-values)
- [Change Texture format](#Change-Texture-format)


## Install

First make sure that the plugin is enabled:
<img width="1136" height="237" alt="image" src="https://github.com/user-attachments/assets/3df3342a-62fc-4b5e-b87e-605ebae5fac4" />

## Vector Field To Volume Texture

Right click on any vector static field, and select **Convert to Volume Texture**. 
<img width="1062" height="326" alt="2026-10-31 15_53_21-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/71798fa3-1d64-46c4-ae68-6881c9e9b049" />

A new Volume Texture will be created in the same folder.
<img width="1447" height="968" alt="DisplayVolume" src="https://github.com/user-attachments/assets/c6fda7e0-9c99-4a25-ba4f-0e082d388d90" />


## Sparse Volume Texture to Volume Texture

Right click on any Sparse Volume Texture, select **Convert to Dense Volume Texture**.

You'll have the option to choose from Attribute A or B, to convert just the first channel (R) or first three (RGB) or all channels. If you right clicked an animated Sparse Volume Texture, you can also select which frame you want to convert.

<img width="424" height="327" alt="2026-11-02 11_17_57-Convert Sparse Volume Texture to Dense" src="https://github.com/user-attachments/assets/d3aa1409-a4e3-4eec-84c9-02ecea0c0dad" />

You can keep the original size, or downsize to some cubic sizes. When downsizing, you will loose the original volume ratio.
<img width="433" height="384" alt="2026-10-31 15_27_19-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/0e85eef7-6259-44dd-9632-54f137e52556" />

## Modify Texture values

Right click on any Texture (2D or Volume) to change its values, select **Apply Math Expression**. You'll be able to apply math expressions to all values of the texture. The operation can create a new texture or directly change values on the same texture.

Allowed math operations are: `+, -, *, /, ^, (, ), abs, floor, ceil, sqrt, log, exp, pow, min, max, clamp`.

1. <img width="964" height="288" alt="2026-10-31 15_28_09-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/06078e06-46c5-4656-b8f5-5ecdc392129d" />

2. <img width="489" height="258" alt="2026-10-31 15_31_04-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/91376b3a-4c88-45ba-a6f2-57cfee56b8f0" />

3. <img width="232" height="188" alt="2026-10-31 15_31_23-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/f77e3f77-e7c0-49b8-9fa6-54da53e433cb" />

4. Also works on Volume Textures:
<img width="627" height="297" alt="2026-10-31 15_37_16-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/3b85683c-c5d8-428e-b7c2-ed2a706ee851" />


## Change Texture format

You can now change a texture's format by right-clicking on any texture:

<img width="1052" height="288" alt="2026-11-02 11_19_25-SVT_5_7_CPP - Unreal Editor" src="https://github.com/user-attachments/assets/d09bd27d-059e-4ea7-a479-0be7958ff68a" />

Select a destination format, depending on the format you might have some additional options. The change can happen in place or in a new texture (default).

<img width="420" height="276" alt="2026-11-02 11_19_56-Change Texture Format" src="https://github.com/user-attachments/assets/9fca0921-37e6-47bb-a75d-b3c1e10c2201" />



## The end

Enjoy.
