# 3D-GS Viewer Setup
Set up the official 3D-GS SIBR viewer locally and run trained models 

## Prerequisites

1.  **Windows Operating System**
2.  **NVIDIA GPU**
3.  **Up-to-date NVIDIA GPU Drivers:** 
4.  **(Skip-and-try) Microsoft Visual C++ Redistributables:** Most Windows systems have these. If the viewer fails to launch with a missing DLL error, you might need to install the latest "Visual C++ Redistributable for Visual Studio 2015-2019" from the [Microsoft website].
## Setup and Viewing Instructions

**Step 1: Download the SIBR Pre-built Viewers**

*   Download the viewers from the official 3D Gaussian Splatting project:
    [zip file](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/binaries/viewers.zip)

    Extract the Zip File in a new folder. 
  
**Step 2: Download a Trained Model**

*   Download from: [Trained-model-of-Truck-1](https://drive.google.com/drive/folders/1kuSjaEOcEjccr4YtQdIOofvsQK1YZPiI?usp=drive_link)
*   Alternatively, if you train your own model, or download pre-trained ones from [official-website](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/) or [click here (Approx.8GB)](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/evaluation/images.zip) you can use that too. 

**Step 3: Run the Viewer**

1.  **Open PowerShell or Command Prompt.**
2.  **Navigate to the `bin` directory of the extracted SIBR viewers:**
    ```powershell
    cd "C:\Path\To\Your\Extracted\Viewers\bin"
    ```

3.  **Run the viewer application, pointing it to the trained model directory:**
    ```powershell
    .\SIBR_gaussianViewer_app.exe -m "C:\Path\To\Your\ae542f1e-6 or folder name"
    ```

## Step 5: Navigate in the Viewer

*   A new window should open displaying the 3D truck scene.
*   **Navigation Controls:**
    *   **Translate Camera:** `W` (forward), `A` (left), `S` (backward), `D` (right), `Q` (down), `E` (up)
    *   **Rotate Camera:** `I` (pitch up), `K` (pitch down), `J` (yaw left), `L` (yaw right), `U` (roll left), `O` (roll right)
*   Explore the floating menus for other options like changing navigation speed or visual settings.
*   **Performance Tip:** For smoother frame rates, disable V-Sync in your NVIDIA Control Panel, and in the viewer application (usually under a "Display" or "Render" menu).

---
