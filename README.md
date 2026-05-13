# CHIL XYZ Capture Grid Calculator

![Capture Grid Calculator UI](./Main-Screen.png)

A standalone, interactive planning tool for automated XYZ table macro photography and high-resolution heritage digitization. 

When imaging oversized archival materials (like maps, manuscripts, and large folios), calculating the exact physical motion grid for an automated XYZ table is critical. This calculator instantly computes the necessary 1:1 Field of View (FOV), motor step sizes, and capture arrays to ensure exact overlap for stitching software like PTGui.

## 🚀 Features

* **Zero-Dependency:** Runs entirely locally in the browser. No installation, build steps, or external servers required. Perfect for isolated lab environments.
* **Camera Sensor Presets:** Built-in exact pixel dimensions for high-end digital backs:
  * Phase One IQ4 150MP (14,204 × 10,652)
  * Phase One IQ3 100MP (11,608 × 8,708)
  * Sony 60MP (9,504 × 6,336)
* **Real-Time Calculation:** Instantly translates target PPI into Pixels-per-Centimeter (PPC) and physical FOV.
* **Step Distance Logic:** Calculates the exact physical distance the camera must travel between shots based on your required overlap percentage.
* **Visual Grid Blueprint:** Provides an immediate visual representation of the capture array and outputs the precise number of columns, rows, and total shots required for the capture sequence.

## 🧮 How It Works (The Math)

The calculator uses standard digitization formulas to guarantee edge-to-edge coverage:

1. **Pixels per cm (PPC):** `PPI / 2.54`
2. **Field of View (FOV):** `Sensor Pixels / PPC`
3. **Step Distance:** `FOV × (1 - Overlap Percentage)`
4. **Grid Array:** `⌈(Object Size − FOV) / Step Distance⌉ + 1`

## 🛠 Usage

1. Clone this repository or download the source code.
2. Open the `.html` file in any modern web browser (Chrome, Firefox, Safari, Edge).
3. Select your camera sensor.
4. Input your target PPI and the physical dimensions of the object in centimeters.
5. Adjust the overlap percentage to fit your stitching tolerance (typically 20-30% for PTGui).
6. Program your automated XYZ table controller with the resulting Step Distances and Grid Array (Columns × Rows).

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. You are free to use, modify, and distribute this tool within your own imaging workflows.
