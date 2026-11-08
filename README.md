[README.md](https://github.com/user-attachments/files/34538342/README.md)
# Cinematic PowerGrade Architect

An AI skill for analyzing cinematic references and designing
professional, reusable DaVinci Resolve PowerGrade workflows.

## Overview

Cinematic PowerGrade Architect helps turn a visual reference into a
structured color-grading plan. It can analyze reference images and
accessible DaVinci Resolve files, describe the look, design a node tree,
and provide practical node-by-node grading instructions.

It is intended for filmmakers, editors, and colorists working on wedding
films, commercials, music videos, and other cinematic projects.

## Features

-   **Reference analysis:** Examine palette, exposure, contrast, white
    balance, skin tones, highlights, shadows, and saturation.
-   **DRX and DPX-aware workflow:** Use supplied DaVinci Resolve `.drx`
    grades and `.dpx` frames when their contents are accessible.
-   **Node-tree design:** Build clear, logical node structures that
    separate technical corrections from creative look development.
-   **Color management:** Account for workflows such as DaVinci Wide
    Gamut / DaVinci Intermediate and Rec.709.
-   **Cinematic look development:** Create warm wedding looks,
    film-inspired aesthetics, moody grades, teal-and-orange looks, and
    natural commercial color.
-   **Practical grading guidance:** Provide node purposes, tool choices,
    suggested adjustments, and validation checks.
-   **Reusable workflows:** Help make grades adaptable across shots,
    cameras, and lighting conditions.

## Workflow

1.  **Provide references** --- Upload a reference image, graded DPX
    frame, DRX file, or original footage/frame when supported.
2.  **Analyze the look** --- Identify the visual characteristics and
    distinguish observations from assumptions.
3.  **Confirm technical context** --- Supply camera, input color space,
    timeline color space, and output requirements when known.
4.  **Build the node tree** --- Plan an ordered grading pipeline
    appropriate to the project.
5.  **Set up each node** --- Receive practical instructions and clearly
    labeled starting points.
6.  **Validate** --- Check skin tones, highlight detail, shadow detail,
    saturation, shot consistency, and output color space.
7.  **Save in Resolve** --- Follow the provided instructions to save or
    export the finished grade as a PowerGrade.

## Example Node Structure

The following is a starting point, not a fixed template. Adapt it to the
project's color-management pipeline and avoid duplicate transforms.

1.  Input color-space transform, if required
2.  Exposure and white balance
3.  Contrast and tonal shaping
4.  Primary color balance
5.  Skin-tone refinement
6.  Creative look development
7.  Color separation and palette shaping
8.  Film texture or finishing effects, if appropriate
9.  Output color-space transform, if required

## Supported Grading Tools

-   Primaries and Log wheels
-   Custom curves
-   Hue vs. Hue
-   Hue vs. Saturation
-   Hue vs. Luminance
-   Color Warper
-   HDR wheels
-   Qualifiers and Power Windows
-   Film grain, glow, and halation when appropriate

## Example Use Prompt

> Analyze this reference image and create a cinematic wedding PowerGrade
> workflow for DaVinci Resolve. Describe the palette, contrast, skin
> tones, highlights, and shadows. Then design a reusable node tree and
> provide node-by-node setup instructions. Clearly identify assumptions
> and do not invent exact settings that cannot be derived from the
> reference.

## Important Notes

-   A reference image shows the appearance of a grade; it does not
    reveal every underlying node setting.
-   Do not blindly copy RGB values from a reference.
-   Keep technical corrections separate from creative look development.
-   Preserve natural skin tones and image detail.
-   Do not assume camera gamma, gamut, or project color management if
    they have not been provided.
-   Distinguish verified settings from visual observations and estimated
    starting points.
-   A working `.drx` file should only be claimed as created when it has
    actually been generated and validated in DaVinci Resolve.

## Requirements

Use with an AI environment that supports custom skill or instruction
files and can inspect the reference materials you provide. DaVinci
Resolve is required to build, test, and save the resulting grade as a
native PowerGrade.

## Author

**Mayur Gawade**

Filmmaking · Photography · DI Color Grading · Creative Technology
