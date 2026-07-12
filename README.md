# PCB Business Card

> A business card created in KiCad utilizing the silkscreen and exposed copper layers for a dual tone effect. Has reference equations and footprints on one side and business card info on the other.

<p align="center">
  <img src="/assets/pcb_business_card_front.png" width="400" alt="Front render, reference side">
  <img src="/assets/pcb_business_card_back.png" width="400" alt="Back render, business card side">
</p>

## Table of Contents

- [Overview](#overview)
- [Design](#design)
- [Manufacturing](#manufacturing)
  - [Panelization](#panelization)
  - [PCB Design](#pcb-design)
- [Bill of Materials](#bill-of-materials)
- [Author](#author)
- [License](#license)

## Overview

This card is a small side project built to double as both a functional reference sheet and a business card. Instead of printing on paper, the whole thing lives on a PCB. One face is packed with the formulas, footprints, and color codes I reach for most often on the bench. The other is a straight up business card with contact info and a quick summary of my skill set, backed by QR codes linking out to GitHub and Printables.

The dual tone look comes from the contrast between the white silkscreen ink and the bare gold exposed copper underneath, so no paint or extra process is needed to get a two color card off a standard fab run.

## Design

Photos of both sides are above. The front is a bench reference sheet featuring an Ohm's law wheel, resistor color code, SMD package sizes, common footprints, LED wavelength chart, and watt color code. The back is the actual business card, mirrored on the second card in the panel so both read correctly once separated.

The dual tone look comes from the contrast between the white silkscreen ink and the bare gold exposed copper underneath, so no paint or extra process is needed to get a two color card off a standard fab run.

## Manufacturing

### Panelization

The panel holds two cards, joined by a perforated snap break rather than a V-score or mouse bites. The perforated snap keeps tooling costs down and gives a clean enough edge for a card that is meant to live in someone's wallet, without paying for a V-scored panel. Two cards per panel also provides the best cost per board on most fabrication quotes, since panel area and minimum order quantities favor larger batches over single small boards.

### PCB Design

Designed in KiCad. All project files are in [`/hardware/kicad_project_files`](/hardware/kicad_project_files).

| Property | Detail |
|----------|--------|
| Layers | 2-layer |
| Finish | ENIG (for the gold exposed copper contrast) |
| Solder Mask | None over the exposed copper regions used for the dual tone artwork |
| Silkscreen | White, used for text and line art on both sides |
| Panel | 2-up, perforated snap break |

## Bill of Materials

| Item | Qty | Unit Cost | Total |
|------|----:|----------:|------:|
| PCB Panels (2 cards each) | 10 | $3.64 | $36.37 |
| **Cost per card** | 20 | **$1.82** | |

> - Total includes shipping. Order was 10 panels, yielding 20 cards total.
> - Most of the per-unit cost comes from the ENIG finish, which gives the exposed copper its gold color for the dual tone effect. A HASL finish would reduce the cost significantly but sacrifice that appearance.
> - No components are assembled; the card is bare PCB only.

## Author

**Seth Hibpshman**

Student of Electrical Engineering, Eastern Washington University

## License

[GNU General Public License v3.0](LICENSE)
