# Wildlife In Focus

![Wildlife In Focus prototype](media/weepaws_preview.gif)

An interactive exhibit at the **California Science Center** — its first fully in-house exhibit — that turns citizen-science data into a personal encounter with the wildlife in a visitor's own area.

Visitors enter their location at a kiosk and the piece pulls citizen-science photos from [iNaturalist](https://www.inaturalist.org/) of animals that live near them. As the experience runs, animated paw prints cross the screen; when they reach the right edge, a camera shutter sound plays from a speaker in the right-hand wall, directing the visitor's attention to a large wall projection. There, the local animals are presented as if they were photographs, and a human silhouette appears — inviting the visitor into a selfie moment with the animal imagery.

## From Prototype to Production

This repo is the prototype behind Wildlife In Focus, developed as part of the design and development process for the finished experience at the California Science Center.

The prototype worked out the interaction, the real-time visual behavior, and the technical approach that were then developed into a public-facing museum installation. The finished experience integrates real-time software with physical exhibit hardware and audiovisual systems, and is designed for continuous operation by thousands of museum visitors.

**My role:** I led the technical and creative development of the interactive, working with my team to move the concept from prototype through implementation, installation, testing, and ongoing operation.

### Prototype

The clip above shows the prototype and demonstrates the underlying interaction and visual system. It set out to answer three questions before anything was built for the gallery floor:

- **Interaction flow** — can a kiosk, a moving on-screen cue, a sound from the wall, and a projection read as one continuous experience across a physical space?
- **Real-time visual behavior** — how do local wildlife photos, paw-print motion, and the silhouette moment behave on screen and on the wall?
- **Data integration** — how do a visitor's location and live iNaturalist data drive what they see?

### Production

The production version required substantial work beyond the prototype:

- Integration with exhibit hardware
- Deployment on dedicated computers
- Audiovisual integration
- Network configuration
- Reliability testing
- Startup and recovery procedures
- Documentation for long-term museum operation

### What this demonstrates

This project is representative of my work at the intersection of creative technology, interaction design, real-time systems, and physical experience design: taking an experimental interactive concept and turning it into a reliable public installation.

- **Prototyping and interaction design** — proving out an experience before committing to build it
- **Real-time systems** — TouchDesigner-based visuals, audio cues, and data-driven content
- **Systems integration** — software, exhibit hardware, audiovisual gear, and networks working as one system
- **Operational reliability** — built for continuous public use, with recovery procedures and handoff documentation
- **Technical leadership** — leading a team from concept through installation and ongoing operation

## Prototype files

- `PhotoArc_ServerDemo.toe`, `PhotoArc_res.toe`, `WallProjectorMount.toe`, `MorphPaws2Feet.toe`, `PhotoArc.toe` — the prototype's TouchDesigner network (kiosk logic, iNaturalist data handling, wall projection output, paw-print animation)
- `Arctext.tox` — custom text/UI component
- [`wif-fronds/`](wif-fronds/) — a related generative visual sub-piece (multiple stripe/speckle/frond variations)
- [`weepaws/`](weepaws/) — the paw-print and bird animation components

The production system's software, configuration, and hardware integration are not included in this repository.

## Requirements

- [TouchDesigner](https://derivative.ca/) (macOS)

## Media

GIF previews are in each folder's `media/` directory — original render exports were excluded for size.
