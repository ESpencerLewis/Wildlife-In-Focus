# Photo Arc

![preview](media/weepaws_preview.gif)

An interactive kiosk exhibit built in TouchDesigner — the first in-house exhibit produced at the **California Science Center**.

Visitors enter their location at a kiosk and the piece pulls citizen-science photos from [iNaturalist](https://www.inaturalist.org/) of animals that live in their area. As the experience runs, animated paw prints cross the screen; when they reach the right edge, a camera shutter sound plays from a speaker in the right-hand wall, directing the visitor's attention to a large wall projection. There, the local animals are presented as if they were photographs, and a human silhouette appears — inviting the visitor into a selfie moment with the animal imagery.

## Structure

- `PhotoArc_ServerDemo.toe`, `PhotoArc_res.toe`, `WallProjectorMount.toe`, `MorphPaws2Feet.toe`, `PhotoArc.toe` — the exhibit's core TouchDesigner network (kiosk logic, iNaturalist data handling, wall projection output, paw-print animation)
- `Arctext.tox` — custom text/UI component
- [`wif-fronds/`](wif-fronds/) — a related generative visual sub-piece (multiple stripe/speckle/frond variations) used within the exhibit
- [`weepaws/`](weepaws/) — the paw-print and bird animation components

## Requirements

- [TouchDesigner](https://derivative.ca/) (macOS)

## Media

GIF previews are in each folder's `media/` directory — original render exports were excluded for size.
