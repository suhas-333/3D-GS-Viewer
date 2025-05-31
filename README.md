# 3D-GS Viewer Setup
Set up the official 3D-GS SIBR viewer locally and run trained models 

## Prerequisites

1.  **Windows Operating System**
2.  **NVIDIA GPU**
3.  **Up-to-date NVIDIA GPU Drivers:** Ensure your graphics drivers are current. 
4.  **(Potentially) Microsoft Visual C++ Redistributables:** Most Windows systems have these. If the viewer fails to launch with a missing DLL error, you might need to install the latest "Visual C++ Redistributable for Visual Studio 2015-2019" from the [Microsoft website].
## Setup and Viewing Instructions

**Step 1: Download the SIBR Pre-built Viewers**

*   Download the viewers from the official 3D Gaussian Splatting project:
    [https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/binaries/viewers.zip](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/binaries/viewers.zip)

**Step 2: Extract the Viewers**

*   Create a folder on your computer where you want to keep the viewers (e.g., `C:\SIBR_Viewers`).
*   Extract the contents of the downloaded `viewers.zip` file into this folder.
  
**Step 3: Download a Trained Model**

*   This repository contains a pre-trained "truck" model output. Download it.
*   Alternatively, if you trained your own model, note the path to your output directory.

**Step 4: Run the Viewer**

1.  **Open PowerShell or Command Prompt.**
2.  **Navigate to the `bin` directory of the extracted SIBR viewers:**
    ```powershell
    cd "C:\Path\To\Your\Extracted\Viewers\bin"
    ```
    *(Replace `C:\Path\To\Your\Extracted\Viewers\bin` with the actual path from Step 2, e.g., `cd "C:\SIBR_Viewers\bin"`)*

3.  **Run the viewer application, pointing it to the trained model directory:**
    ```powershell
    .\SIBR_gaussianViewer_app.exe -m "C:\Path\To\Your\truck_model_output"
    ```
    *(Replace `C:\Path\To\Your\truck_model_output` with the actual path to the folder containing your trained truck model from Step 3. Remember to use quotes if the path has spaces.)*

**Step 5: Navigate in the Viewer**

*   A new window should open displaying the 3D truck scene.
*   **Navigation Controls:**
    *   **Translate Camera:** `W` (forward), `A` (left), `S` (backward), `D` (right), `Q` (down), `E` (up)
    *   **Rotate Camera:** `I` (pitch up), `K` (pitch down), `J` (yaw left), `L` (yaw right), `U` (roll left), `O` (roll right)
*   Explore the floating menus for other options like changing navigation speed or visual settings.
*   **Performance Tip:** For smoother frame rates, disable V-Sync in your NVIDIA Control Panel, and in the viewer application (usually under a "Display" or "Render" menu).

---
