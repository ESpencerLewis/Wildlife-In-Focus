# Wildlife In Focus

![Wildlife In Focus prototype](media/weepaws_preview.gif)

A permanent interactive exhibit at the **California Science Center** — its first fully in-house exhibit — that turns citizen-science data into a personal encounter with the wildlife in a visitor's own neighborhood.

Visitors enter their address at a kiosk screen. Animal footprints walk across the screen toward a wall, where an attract loop is playing. A camera-shutter sound plays from the projector, and the wall changes to photos of animals from each animal class found in the visitor's ZIP code, arranged around a silhouette that invites them to step in and take a selfie with the wildlife. The animal photos come from [iNaturalist](https://www.inaturalist.org/) citizen-science observations, retrieved by image URL.

## From Prototype to Production

This repo is the prototype behind Wildlife In Focus, developed as part of the design and development process for the finished experience at the California Science Center.

The prototype worked out the interaction, the real-time visual behavior, and the technical approach that were then developed into a public-facing museum installation. The finished exhibit integrates real-time software with physical exhibit hardware and audiovisual systems. It runs every day as a permanent exhibit, for roughly 5,000 visitors a day.

**My role:** I led the technical and creative development of the interactive, working with a team of five to take the concept from prototype through implementation, installation, testing, and ongoing operation. I also maintain the exhibit long-term.

### Prototype

The clip above shows the prototype and demonstrates the underlying interaction and visual system. It set out to answer three questions before anything was built for the gallery floor:

- **Interaction flow** — can a kiosk, a moving on-screen cue, a sound, and a wall projection read as one continuous experience across a physical space?
- **Real-time visual behavior** — how do local wildlife photos, footprint motion, and the silhouette moment behave on screen and on the wall?
- **Data integration** — how do a visitor's address and iNaturalist photo data drive what they see?

### Production

The production system is built from a PC, a Raspberry Pi, a short-throw projector, and a kiosk screen, with photos pulled live from iNaturalist by URL. Getting from prototype to that system required substantial work:

- Integration with exhibit hardware
- Deployment on dedicated computers
- Audiovisual integration
- Network configuration
- Reliability testing
- Startup and recovery procedures
- Documentation for long-term museum operation

At roughly 5,000 visitors a day, every day, the exhibit depends on reliable startup and recovery procedures and has to stay maintainable over years — I own that ongoing maintenance.

### What this demonstrates

This project is representative of my work at the intersection of creative technology, interaction design, real-time systems, and physical experience design: taking an experimental interactive concept and turning it into a reliable public installation.

- **Prototyping and interaction design** — proving out an experience before committing to build it
- **Real-time systems** — a TouchDesigner prototype driving live visuals, audio cues, and data-driven content
- **Systems integration** — a PC, Raspberry Pi, short-throw projector, kiosk screen, audio, and network working as one system
- **Operational reliability** — built for continuous public use, with recovery procedures and handoff documentation
- **Long-term ownership** — maintaining a permanent exhibit after launch, not just building it
- **Technical leadership** — leading a team of five from concept through installation and ongoing operation

## Prototype files

- `PhotoArc_ServerDemo.toe`, `PhotoArc_res.toe`, `WallProjectorMount.toe`, `MorphPaws2Feet.toe`, `PhotoArc.toe` — the prototype's TouchDesigner network (kiosk logic, iNaturalist data handling, wall projection output, footprint animation)
- `Arctext.tox` — custom text/UI component
- [`wif-fronds/`](wif-fronds/) — a related generative visual sub-piece (multiple stripe/speckle/frond variations)
- [`weepaws/`](weepaws/) — the footprint and bird animation components

The production system's software, configuration, and hardware integration are not included in this repository.

## Requirements

- [TouchDesigner](https://derivative.ca/) (macOS)

## Media

GIF previews are in each folder's `media/` directory — original render exports were excluded for size.
