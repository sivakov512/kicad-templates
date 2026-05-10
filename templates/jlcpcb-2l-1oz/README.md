# JLCPCB 2L 1oz

KiCad template for JLCPCB's standard 2-layer board: 1oz copper, 1.6mm, minimum design rules.

---

## Key Features

* ✅ **2-layer, 1oz copper**, 1.6062 mm total thickness
* ✅ Design rule constraints set to **JLCPCB's lowest-cost thresholds**
* ✅ Silkscreen and copper text tuned to **pass fab tolerances**
* ✅ `LCSC PN` field present in schematic for **automated BOM generation**
* ✅ `Default` net class set to JLCPCB minimum clearances
* ✅ `Local` symbol and footprint libraries **pre-connected** for project-specific components

---

## Stackup

| Layer     | Material | Thickness  |
| --------- | -------- | ---------- |
| Top Cu    | Cu       | 0.035 mm   |
| Core      | FR4      | 1.5162 mm  |
| Bottom Cu | Cu       | 0.035 mm   |

**Total thickness**: 1.6062 mm

---

## Design Rules → Constraints

| Parameter                   | Value   |
| --------------------------- | ------- |
| Minimum clearance           | 0.1 mm  |
| Minimum track width         | 0.1 mm  |
| Minimum connection width    | 0.1 mm  |
| Minimum annular width       | 0.05 mm |
| Minimum via diameter        | 0.4 mm  |
| Copper to hole clearance    | 0.2 mm  |
| Copper to edge clearance    | 0.2 mm  |
| Minimum through hole        | 0.3 mm  |
| Hole to hole clearance      | 0.2 mm  |
| Silkscreen → item clearance | 0.15 mm |
| Min text height             | 1 mm    |
| Min text thickness          | 0.15 mm |

---

## Net Classes → `Default`

| Property       | Value   |
| -------------- | ------- |
| Clearance      | 0.1 mm  |
| Track Width    | 0.1 mm  |
| Via Size       | 0.4 mm  |
| Via Hole       | 0.3 mm  |
| DiffPair Width | 0.15 mm |
| DiffPair Gap   | 0.15 mm |

---

## Text & Graphics Defaults

| Layer  | Line Thickness | Text Height | Text Width | Text Thickness |
| ------ | -------------- | ----------- | ---------- | -------------- |
| Silk   | 0.15 mm        | 1 mm        | 1 mm       | 0.15 mm        |
| Copper | 0.2 mm         | 1.5 mm      | 1.5 mm     | 0.3 mm         |

Complies with JLCPCB silkscreen rules: ≥1 mm height, ≥0.15 mm line.

---

## Schematic Setup

* `LCSC PN` field template pre-included for BOM and placement file generation during JLCPCB assembly quoting.

## Local Libraries

`Local` symbol and footprint libraries are pre-connected in `sym-lib-table` and `fp-lib-table`, pointing to `Local.kicad_sym` and `Local.pretty/` inside the project directory.

Add project-specific components there without touching global library tables.

---

## Notes

* No finish, mask or stencil settings enforced — tune them at Gerber export.
