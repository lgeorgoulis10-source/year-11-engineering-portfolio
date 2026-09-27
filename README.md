# year-11-engineering-portfolio
A dual-axis solar tracker integrating OpenCV on Raspberry Pi 5, micro:bit sensor fusion, and custom CAD hardware.
### Design Iteration 1: Sensor Array Head & Clash Detection
The first mechanical challenge was designing a unified mount to house a heavy, non-standard USB webcam alongside two CamJam LDR sensors, driven by a single 9g SG90 tilt servo. 

**Problem 1: Sensor Alignment & FOV**
Initial CAD iterations placed the 5mm LDR holsters on the lateral sides of the mount. I realized this would cause the sensors to face perpendicular to the camera's line of sight, breaking the sensor fusion requirement. 
*   *Solution:* Reoriented the extrusions to the front face so the LDRs and camera share a parallel Field of View (FOV).

**Problem 2: Mechanical Clashing**
The webcam utilizes a 38mm-wide folding laptop clip with a 14mm overhang. If the LDR tubes were centered, the camera clip would physically crash into them during mounting.
*   *Solution:* Iterated the main mounting wall width from 40mm to 60mm. By spacing the 8mm LDR tubes exactly 6mm from the outer edges, I created a clear central channel for the camera clip to lock onto the 10mm-thick wall without interfering with the raw analog light sensors. 

**Tolerances applied:**
*   LDR holsters designed with a 5.2mm inner diameter for a snug friction fit on 5mm components.
*   Bottom servo plate designed with 16mm center-to-center 1.5mm holes to match standard SG90 straight plastic horns.
