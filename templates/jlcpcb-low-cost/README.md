# JLCPCB Low-Cost Template

A production-oriented KiCad template aligned with [JLCPCB's PCB fabrication capabilities](https://jlcpcb.com/capabilities/pcb-capabilities), using minimum design rules for cost-effective prototyping and manufacturing.

The template is preconfigured with a 4-layer stackup and standard low-cost constraints, but you're free to adjust the number of layers as needed.

---

## Key Features

* ✅ Based on **JLCPCB's official capability specs**: [jlcpcb.com/capabilities](https://jlcpcb.com/capabilities/pcb-capabilities)
* ✅ Preconfigured for **4-layer stackup** (total 1.525 mm), easily replaceable with any layer count
* ✅ Design rule constraints set to **JLCPCB's lowest-cost thresholds**
* ✅ Silkscreen and copper text tuned to **pass fab tolerances**
* ✅ `LCSC PN` field present in schematic for **automated BOM generation**
* ✅ `Default` net class mirrors DRC minimums for **dense routing**

---

## Stackup (Default: 4 Layers)

| Layer     | Material | Thickness |
| --------- | -------- | --------- |
| Top Cu    | Cu       | 0.035 mm  |
| Prepreg   | FR4      | 0.1 mm    |
| In1 Cu    | Cu       | 0.0175 mm |
| Core      | FR4      | 1.2 mm    |
| In2 Cu    | Cu       | 0.0175 mm |
| Prepreg   | FR4      | 0.1 mm    |
| Bottom Cu | Cu       | 0.035 mm  |

**Total thickness**: 1.525 mm

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
| uVia diameter               | 0.25 mm |
| uVia hole size              | 0.15 mm |
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
| Via Hole       | 0.4 mm  |
| µVia Size      | 0.25 mm |
| µVia Hole      | 0.15 mm |
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

* `LCSC PN` field template pre-included for part number assignment.
* Useful for automatic BOM and placement file generation during assembly quoting.

---

## Notes

* No finish, mask or stencil settings enforced — tune them at Gerber export.
* Works great as a base for quick prototypes or clean reusable boards.
