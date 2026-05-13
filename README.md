# XYZ Capture Grid Calculator
A standalone interactive grid calculator for our in-house automated XYZ table photography. It instantly computes FOV, motor step sizes, and capture arrays to ensure exact overlap for PTGui stitching.

When digitizing oversized flat objects like maps, archival manuscripts, and large folios, calculating the exact motion grid for an automated XYZ table can be tedious. The CHIL XYZ Capture Grid Calculator is a standalone, interactive utility designed to streamline high-resolution heritage imaging workflows.

By inputting the target object dimensions, desired PPI, and overlap percentage (optimized for software like PTGui), the calculator instantly generates the exact capture array. Built with a focus on high-end digital sensors like the Phase One 100MP back, this tool allows operators to easily translate physical surface areas into precise motor steps.

Key Features:
Real-Time Step Calculation: Translates your target PPI into a 1:1 physical Field of View (FOV) and calculates the exact X/Y distance per move based on your required overlap percentage.

Automated Array Generation: Accurately computes the ceiling limits for required rows and columns (⌈(Object Size − FOV) / Step Size⌉ + 1) to guarantee full edge-to-edge coverage of the object.

Visual Grid Feedback: Provides an immediate visual breakdown of the total shots, columns, and rows required for the job.

Zero-Dependency Deployment: Packaged as a single, fully bundled HTML file. It runs locally in any web browser, making it perfect for isolated lab workstations or offline capture environments.

Use Case
Ideal for digital content units and libraries processing large classmark batches where camera height (PPI) and overlap tolerances must be strictly maintained across hundreds of macro shots.
