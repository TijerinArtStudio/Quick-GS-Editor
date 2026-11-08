# Quick GS Editor

<p align="center">
  <a href="https://www.youtube.com/watch?v=QGs7Jcskne8">
    <img src="https://img.youtube.com/vi/QGs7Jcskne8/maxresdefault.jpg" alt="Watch the Quick GS Editor promotional video" width="100%">
  </a>
  <br>
  <a href="https://www.youtube.com/watch?v=QGs7Jcskne8">▶ Watch the promotional video on YouTube</a>
</p>

<p align="center">
  <strong>A powerful Gaussian Splatting editor for artists, 3D creators, and developers.</strong><br>
  Edit, clean, align, sculpt, and enhance Gaussian Splatting scenes with an extensive set of creative tools.
</p>

<p align="center">
  <a href="https://tijerinart.itch.io/quick-gs-editor">Free Web App</a> ·
  <a href="https://tijerinart.itch.io/quick-gs-editor-full-version">Premium Edition</a> ·
  <a href="https://github.com/TijerinArtStudio/Quick-GS-Editor">GitHub Repository</a>
</p>

---

## Overview

**Quick GS Editor (QGSE)** is a Gaussian Splatting editing suite created by **Tijerín Art Studio**. It is designed to make common and advanced 3D Gaussian Splatting tasks accessible through a focused editing workflow: clean noisy captures, correct geometry, align scenes, modify colors, project textures, fill gaps, and prepare assets for further production.

The free edition runs in the browser and is powered by **Spark, the 3D Gaussian Splatting renderer developed by World Labs**. The Premium Edition adds a standalone workflow and exclusive tools, including local AI-powered generation with **TripoSplat**.

> **Project and engine attribution:** Quick GS Editor is developed by Tijerín Art Studio. Spark is a third-party renderer built by World Labs and used as the rendering technology for the web application. Quick GS Editor is not a World Labs product.

## Editions

| Edition | What it includes |
| --- | --- |
| **Free Web Edition** | Browser-based Gaussian Splatting editor powered by Spark, with the core editing and scene-processing tools described below. |
| **Premium Edition** | A downloadable, standalone version with the free edition's features, additional Premium tools, and offline use. |

### Free Web Edition

Launch Quick GS Editor directly from itch.io:

**[Open Quick GS Editor — Free Web Edition](https://tijerinart.itch.io/quick-gs-editor)**

The web edition uses Spark and runs in a compatible browser. Performance depends on the browser, GPU, and size of the scene being edited.

### Premium Edition

The Premium Edition is available as a downloadable application:

**[Get Quick GS Editor — Premium Edition](https://tijerinart.itch.io/quick-gs-editor-full-version)**

According to the itch.io product page, the Premium Edition includes:

- Every feature available in the free web version.
- Exclusive standalone tools.
- A DRM-free downloadable build.
- Offline use, without recurring online validation.
- Lifetime access to future builds and updates.
- Permission to share the build with collaborators and students, as described on the product page.

Some optional Premium features have their own hardware or setup requirements; see the TripoSplat section below.

## Rendering technology: Spark by World Labs

The free browser edition is powered by **[Spark](https://sparkjs.dev/)**, an open-source 3D Gaussian Splatting renderer developed by **[World Labs](https://www.worldlabs.ai/)**.

Spark is built for Three.js and WebGL2. It provides the rendering foundation for displaying Gaussian Splats in the browser and is designed to support multiple splat objects, dynamic splat operations, and integration with conventional 3D scene content.

A few important distinctions:

- **Spark is the rendering engine; Quick GS Editor is the application.** The editing workflow and product are developed by Tijerín Art Studio.
- World Labs is credited as the creator of Spark, not as the developer or publisher of Quick GS Editor.
- Spark is an independent open-source project. See its [official GitHub repository](https://github.com/sparkjsdev/spark) for its source code, documentation, and license.
- The browser edition relies on WebGL2 support. Actual performance varies with the device and the complexity of the Gaussian Splatting scene.

## Features

### Multiply — intelligent splat densification

Fill sparse areas and small holes by interpolating new splats from their neighbours. Multiply is designed to reinforce existing surfaces and improve density without simply inventing unrelated detail.

![Multiply tool demonstration](https://img.itch.zone/aW1nLzMxOTc5NzcyLmdpZg%3D%3D/original/jzRZjV.gif)

### Area Masks and Gradients

Use box-shaped or spherical volumetric areas to control parts of a scene. Apply gradients and geometric masks to blend multiple Gaussian clouds, isolate regions, crop unwanted areas, and prepare a cleaner, lighter export.

![Area Masks and Gradients demonstration](https://img.itch.zone/aW1nLzMxOTc5ODE4LmdpZg%3D%3D/original/2P5uQT.gif)

### Project — camera-based texture projection

Project solid textures or alpha-masked images onto Gaussian Splats from the current camera view. Use external images or viewport snapshots to cover imperfections such as stains, cracks, sockets, and scanning artifacts.

![Project tool demonstration](https://img.itch.zone/aW1nLzMxOTc5ODQwLmdpZg%3D%3D/original/UDJe1r.gif)

### Brush and Lasso Selection

Select splat clusters directly in the 3D viewport using brush-based or freeform lasso selection. This makes it possible to isolate specific parts of a scene before applying local edits or cleanup operations.

![Brush and Lasso Selector demonstration](https://img.itch.zone/aW1nLzMxOTc5ODU3LmdpZg%3D%3D/original/y1xy1K.gif)

### Clone Stamp

Copy detail from one region and stamp it into another. The Clone tool is useful for repairing damaged areas, repeating existing surface detail, and replacing unwanted parts of a scan in a controlled way.

![Clone Stamp demonstration](https://img.itch.zone/aW1nLzMxOTc5OTkwLmdpZg%3D%3D/original/amMpFY.gif)

### Splat Editing — color, opacity, and scale

Adjust hue, saturation, brightness, opacity, and splat scale. Apply changes to the whole Gaussian cloud or restrict them to selected splats for localized corrections.

![Splat Editing demonstration](https://img.itch.zone/aW1nLzMxOTc5ODkyLmdpZg%3D%3D/original/tWH5zf.gif)

### Alignment Tools

Level the ground axis with a single operation and align one Gaussian Splat scene with another. These tools help prepare captures for composition and make it easier to combine separate scans in a shared scene.

![Alignment tools demonstration](https://img.itch.zone/aW1nLzMxOTc5OTAwLmdpZg%3D%3D/original/Zc4X4e.gif)

### Clean — remove unwanted splats

Prune unwanted points using color, scale, or opacity thresholds. Clean is intended to remove floaters, background noise, and stray splats while reducing the point count and final file size.

![Clean tool demonstration](https://img.itch.zone/aW1nLzMxOTgwMDAwLmdpZg%3D%3D/original/4a%2BQPV.gif)

### Sculpt — edit the shape of a splat cloud

Deform and manipulate splat volumes with brush-based sculpting. Use it to correct geometry, refine silhouettes, and polish shapes at both large and small scales.

![Sculpt tool demonstration](https://img.itch.zone/aW1nLzMxOTgwODQ1LmdpZg%3D%3D/original/732FyA.gif)

### More Gaussian Splatting workflows

Quick GS Editor also brings together additional production workflows, including:

- Merging multiple Gaussian clouds.
- Working with dynamic 4D Gaussian Splatting animations on a timeline.
- Converting polygonal 3D meshes into Gaussian Splats.
- Converting or processing splat clouds into fully textured 3D assets.
- Recoloring splats according to camera depth.

![Additional Quick GS Editor workflows](https://img.itch.zone/aW1nLzMxOTc5ODI1LmdpZg%3D%3D/original/ydBDcn.gif)

## Premium tools

The Premium Edition includes additional standalone tools that are not part of the free web edition.

### Real-Time Fluid Simulation — experimental

Simulate particle-based fluid dynamics with customizable physics. Bake simulations onto the timeline and export individual frames as sequential PLY files for use in external DCC applications.

This feature is marked as **experimental**.

![Premium Fluid Simulation demonstration](https://img.itch.zone/aW1nLzMxOTgwMDEyLmdpZg%3D%3D/original/3OI9t2.gif)

### TripoSplat — local AI Gaussian Splat generation

The Premium Edition includes **TripoSplat**, a local AI generation tool that creates optimized Gaussian Splats from a single source image.

- Runs locally from inside the standalone application.
- Includes a one-click installation workflow.
- Initial setup requires an internet connection.
- An **NVIDIA GPU** is required.
- After the initial setup, generation runs locally and can be used offline.

**Naming note:** the current itch.io product description calls this feature **TripoSplat**. That is the name used in this README.

![TripoSplat demonstration](https://img.itch.zone/aW1nLzMxOTgwMDIxLmdpZg%3D%3D/original/%2BAshEM.gif)

### Reflect Engine — environment reflections

Inject custom Spherical Harmonics (SH) into Gaussian Splats using 360° environment HDRI panoramas. Control roughness and highlight placement to create more accurate specular highlights and environment reflections.

![Reflect Engine demonstration](https://img.itch.zone/aW1nLzMxOTgwMDQyLmdpZg%3D%3D/original/qLpliS.gif)

## Who is Quick GS Editor for?

Quick GS Editor is intended for:

- **3D artists** who need to clean, refine, and prepare Gaussian Splatting captures.
- **Photogrammetry and scanning workflows** that need artifact removal, alignment, and local corrections.
- **Environment artists** who want to combine scans, fill gaps, or project textures onto splat scenes.
- **Developers and technical artists** who need to prepare Gaussian Splatting assets for interactive projects.
- **AI-assisted 3D workflows** that use generated or reconstructed Gaussian Splatting content.

## Links

- **Free Web Edition:** https://tijerinart.itch.io/quick-gs-editor
- **Premium Edition:** https://tijerinart.itch.io/quick-gs-editor-full-version
- **Promotional video:** https://www.youtube.com/watch?v=QGs7Jcskne8
- **Spark — official website:** https://sparkjs.dev/
- **Spark — source repository:** https://github.com/sparkjsdev/spark
- **Developer:** https://tijerinart.itch.io/

## Credits and third-party technology

Quick GS Editor is created and maintained by **Tijerín Art Studio**.

**Spark** is developed by **World Labs** and is used as the rendering technology for the free browser edition. Spark is a separate open-source project; its code, documentation, and licensing terms are maintained in the [official Spark repository](https://github.com/sparkjsdev/spark).

Product names and trademarks mentioned in this README belong to their respective owners.
