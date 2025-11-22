# Day 1 Theory Notes - USD Quickstart
Date: November 22, 2025

## What USD Is
- A 3D file format and API created by Pixar  
- A new standard for storing scene information
- Developed by Pixar during Brave (2010) to solve data exchange issues
- Open-sourced in 2016, used in films and industries like automotive
- Assets are built from smaller USD files (geometry, materials, textures)
- Files reference each other, forming a tree-like hierarchy

### Folder and File Structure
- Geometry, materials, and textures stored separately
- Each file is lightweight and editable, enabling version control and overrides

## Why USD Is Different
- Instead of one bloated file, USD describes how to assemble a scene from smaller files
- Improves performance and allows selective loading of assets
- Enables vehicle variants (tractor, sedan, ambulance)

## Industry Need
- Modern productions involve multiple major VFX houses and diverse software
- USD acts as a "holy grail" for seamless data exchange

## Core Concepts Learned:

### Stage
- USD uses "stages" to assemble scenes from assets
- Layers allow hierarchical "opinions" that override but don't overwrite lower layers
- Layout, animation, FX, and lighting each add their own layers
- Artists can mute or override changes from other departments
- Everyone works from one central dataset, avoiding conflicting versions
- Enables non-destructive editing and collaboration across departments

### Prim
- Prims are the smallest units in USD (could be a kettle or its parts)
- They differ from Maya polygons and can't be broken down further

### Variants and Flexibility
- Prims can have alternate versions called variants
- Artists must plan how to break down objects into prims before exporting
