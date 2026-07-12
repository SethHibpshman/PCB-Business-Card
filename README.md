\# PCB Business Card



> A business card created in KiCad utilizing the silkscreen and exposed copper layers for a dual tone effect. Has reference equations and footprints on one side and business card info on the other.



<p align="center">

&#x20; <img src="/assets/pcb\_business\_card\_front.png" width="400" alt="Front render, reference side">

&#x20; <img src="/assets/pcb\_business\_card\_back.png" width="400" alt="Back render, business card side">

</p>



\## Table of Contents



\- \[Overview](#overview)

\- \[Design](#design)

\- \[Manufacturing](#manufacturing)

&#x20; - \[Panelization](#panelization)

&#x20; - \[PCB Design](#pcb-design)

\- \[Bill of Materials](#bill-of-materials)

\- \[Author](#author)

\- \[License](#license)



\## Overview



This card is a small side project built to double as both a functional reference sheet and a business card. Instead of printing on paper, the whole thing lives on a PCB. One face is packed with the formulas, footprints, and color codes I reach for most often on the bench. The other is a straight up business card with contact info and a quick summary of my skill set, backed by QR codes linking out to GitHub and Printables.



The dual tone look comes from contrast between the white silkscreen ink and the bare gold exposed copper underneath, so no paint or extra process is needed to get a two color card off a standard fab run.



\## Design



Photos of both sides are above. The front is a bench reference sheet (Ohm's law wheel, resistor color code, SMD package sizes, common footprints, LED wavelength chart, watt color code). The back is the actual business card, mirrored on the second card in the panel so both read correctly once separated.



The dual tone look comes from contrast between the white silkscreen ink and the bare gold exposed copper underneath, so no paint or extra process is needed to get a two color card off a standard fab run.



\## Manufacturing



\### Panelization



The panel holds two cards, joined by a perforated snap break rather than a v-score or mousebite. Perf snap keeps tooling cost down and gives a clean enough edge for a card that is going to live in someone's wallet, without paying for a v-scored panel. Two cards per panel also gets the best cost per board on most fab quotes, since panel area and minimum order quantities favor larger batches over single small boards.



\### PCB Design



Designed in KiCad. All project files are in \[`/hardware/kicad\_project\_files`](/hardware/kicad\_project\_files).



| Property | Detail |

|---|---|

| Layers | 2 layer |

| Finish | ENIG (for the gold exposed copper contrast) |

| Solder Mask | None over the exposed copper regions used for the dual tone art |

| Silkscreen | White, used for text and line art on both sides |

| Panel | 2-up, perforated snap break |



\## Bill of Materials



| Item | Qty | Unit | Total |

|---|---|---|---|

| PCB Panels (2 cards each) | 10 | $3.64 | $36.37 |

| \*\*Cost per card\*\* | 20 | \*\*$1.82\*\* | |



> - Total includes shipping. Order was 10 panels, 20 cards total.

> - Most of the per unit cost comes from the ENIG finish, which is what gives the exposed copper its gold color for the dual tone effect. A HASL finish would cut cost significantly but trade away that look.

> - No components are assembled; the card is bare PCB only.



\## Author



\*\*Seth Hibpshman\*\*

Student of Electrical Engineering, Eastern Washington University



\## License



\[GNU General Public License v3.0](LICENSE)

