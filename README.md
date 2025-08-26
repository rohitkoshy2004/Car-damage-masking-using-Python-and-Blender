# 🚗 Blender Car Damage Masking
Synthetic Data Generation Using Blender and python. Read # Documentation File before going into it
This project demonstrates how to add **realistic car damage** (dents, scratches, dirt, and cracks) in **Blender** using assets, procedural textures, and a Python script.

---

## 📌 Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Importing the Car Model](#importing-the-car-model)
- [Importing Assets](#importing-assets)
- [Running the Python Script](#running-the-python-script)
- [Changing the Mode Switcher Node](#changing-the-mode-switcher-node)
- [Creating Damages](#creating-damages)
- [Applying Dirt Texture](#applying-dirt-texture)
- [Applying the HDRI Dome](#applying-the-hdri-dome)
- [Generation](#generation)
- [Unresolved Challenges](#unresolved-challenges)
- [Specific Problems](#specific-problems)
- [Resources](#resources)

---

## 📖 Introduction
This guide walks you through the process of **adding damage masks** (dents, scratches, cracks, dirt) to a car model in Blender.  
The workflow uses:
- Blender shaders & assets  
- A custom **Python script**  
- Rendering with **Cycles Engine**

---

## ⚙️ Prerequisites
- Blender **4.1+** installed  
- Car model file (download or import from BlenderKit)  
- Render engine: **Cycles**  
- Assets available via **Blender Asset Browser**  

---

## 🚙 Importing the Car Model
You have two options:

### **Option 1: Import from File**
1. Open Blender  
2. Go to `File > Import` and select your car model format  
3. Import it into Blender  

### **Option 2: Using BlenderKit Addon**
1. Download and install the **BlenderKit addon**  
2. Enable it in `Edit > Preferences > Add-ons`  
3. Search for **"Car"** in BlenderKit  
4. Click to import into your scene  

---

## 🎨 Importing Assets
1. Open the **Asset Browser**  
2. Drag & drop desired assets (scratches, dents, textures) onto the car model  

---

## 🐍 Running the Python Script
1. Switch to the **Scripting workspace**  
2. Run the provided Python script (link in resources)  

---

## 🔄 Changing the Mode Switcher Node
1. Open the **Shading tab > Shader Editor**  
2. Locate the **Mode Switcher node**  
3. Replace it with the latest version if missing  

---

## 🛠️ Creating Damages
- **Dents** → Adjust `Voronoi Texture` + `Mapping` node scales  
- **Scratches** → Modify values in mapping nodes  
- **Glass Cracks** → Add crack texture nodes  

---

## 🌫 Applying Dirt Texture
Follow this tutorial:  
[Simple Dirt & Dust in Blender](https://www.youtube.com/watch?v=example) 

---

## 🌎 Applying the HDRI Dome
- Use a **dome HDRI** instead of world HDRI  
- Benefits: Keeps car aligned with ground plane  
- Tutorial: [HDRI Dome Tutorial](https://www.youtube.com/watch?v=example&t=363) *(6:03 - 17:38)*  

---

## 🖼️ Generation
1. Set the number of samples  
2. Click **Generate** to render and save  

---

## ⚠️ Unresolved Challenges
- Needs **better procedural dents & scratches**  
- Lighting doesn’t always match background  
- Dents only randomize on one side  
- Car reflections need improvement  

---

## 🐞 Specific Problems
- HDRI environment lacks detailing  
- Geometry nodes need refinement  
- Poor placement of dents  

---

## 📚 Resources
- **Texture resource:** [Click Here](#)  
- **Car Models:**  
  - [Google Drive Collection](https://drive.google.com/drive/folders/1pdVvE4Iy5UDwf-opVEpgLbMOX85w-kB3?usp=drive_link)  
  - [Sketchfab](https://sketchfab.com/categories/cars-vehicles)  
  - [Free3D](https://free3d.com/3d-models/vehicles)  
  - [TurboSquid](https://www.turbosquid.com/3d-model/free/car)  

---

## 🏁 Conclusion
This project serves as a **foundation for procedural car damage simulation** in Blender.  
Future improvements include better node setups, more realistic materials, and enhanced geometry-based denting.  
