# Home Etch Photoresist Template

A KiCad template optimized for home PCB fabrication using photoresist etching methods, configured with design rules suitable for DIY PCB manufacturing with standard photoresist processes and ferric chloride etching.

The template is preconfigured as a 2-layer board with constraints appropriate for home etching capabilities, ensuring reliable results with common DIY equipment and materials.

---

## Key Features

* ✅ Optimized for **home photoresist etching** with UV exposure and chemical etching
* ✅ **2-layer stackup** (1.525 mm total thickness) suitable for standard FR4 blanks
* ✅ Design rules set for **reliable home fabrication** with standard equipment
* ✅ Track widths and clearances tuned for **photoresist resolution limits**
* ✅ Via sizes compatible with **manual drilling** or basic CNC equipment
* ✅ Conservative constraints to ensure **high success rate** in home workshop

---

## Stackup (2 Layers)

| Layer     | Material | Thickness |
| --------- | -------- | --------- |
| Top Cu    | Cu       | 0.035 mm  |
| Core      | FR4      | 1.435 mm  |
| Bottom Cu | Cu       | 0.035 mm  |
| Mask      | -        | 0.01 mm   |

**Total thickness**: 1.525 mm (standard single-sided FR4 blank thickness)

---

## Design Rules → Constraints

| Parameter                   | Value   | Notes                                    |
| --------------------------- | ------- | ---------------------------------------- |
| Minimum clearance           | 0.2 mm  | Safe for photoresist resolution          |
| Minimum track width         | 0.3 mm  | Reliable with standard UV exposure       |
| Minimum connection width    | 0.25 mm | Ensures good electrical connection       |
| Minimum annular width       | 0.25 mm | Adequate for manual drilling tolerance   |
| Minimum via diameter        | 0.8 mm  | Suitable for 0.3 mm drill bits          |
| Copper to hole clearance    | 0.3 mm  | Accounts for drilling precision          |
| Copper to edge clearance    | 0.5 mm  | Safe margin for cutting/routing          |
| Minimum through hole        | 0.3 mm  | Standard drill bit availability          |
| Hole to hole clearance      | 0.3 mm  | Prevents drill breakage                  |
| Min text height             | 0.8 mm  | Readable after etching process           |
| Min text thickness          | 0.08 mm | Maintains legibility                     |

---

## Net Classes → `Default`

| Property       | Value   |
| -------------- | ------- |
| Clearance      | 0.2 mm  |
| Track Width    | 0.3 mm  |
| Via Size       | 0.8 mm  |
| Via Hole       | 0.3 mm  |
| DiffPair Width | 0.2 mm  |
| DiffPair Gap   | 0.25 mm |

---

## Manufacturing Process Compatibility

* **Photoresist**: Optimized for positive photoresist film or spray application
* **UV Exposure**: Track/clearance sizes suitable for standard UV LED exposure boxes
* **Etching**: Compatible with ferric chloride, ammonium persulfate, or muriatic acid + hydrogen peroxide
* **Drilling**: Via and hole sizes match common PCB drill bit sets (0.3-3.0 mm)
* **Surface Finish**: Template assumes bare copper (no plating required)

---

## Notes

* No solder mask or silkscreen layers configured — silkscreen errors are ignored as this layer is not used in home etching
* Conservative design rules prioritize manufacturing success over density
* Test your specific photoresist/exposure setup with simple test patterns first
* Consider tinning traces after etching to prevent oxidation
