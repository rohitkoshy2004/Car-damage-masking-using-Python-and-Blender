# Car-damage-masking-using-Python-and-Blender
Synthetic Data Generation Using Blender and python. 

#Table of Contents
Introduction
Prerequisites
Importing the Car Model
Importing Assets and Applying Them to the Car Model
Running the Python Script
Changing the Mode Switcher Node
Creating Damages
Applying Dirt Texture
Applying the HDRI Dome
Generation
Unresolved Challenges
Specific Problems
Resources

1. Introduction
This documentation will walk you through the process of adding realistic damage, like dents and scratches, to a car model using Blender. 
In this project, we'll use a Blender script to create these damage masks and then render the results, saving them neatly into a folder on your PC.
2. Prerequisites
Blender Installed: Blender version 4.1 or above.
Car Model File:  Any car models.You can import it from online
Render Engine: This project uses Cycles as the render engine.
Assets: Assets can browsed through asset browser
	

3. Importing the Car Model
You have two options to import your car model:
Option 1: Import from File
Open Blender.
Go to File > Import and select the format of your car model.
Navigate to the car model file and import it into Blender.
Option 2: Using BlenderKit Addon
Download the BlenderKit addon: BlenderKit. A zip file is also included in the folder provided.
Open Blender.
Go to Edit > Preferences (or press Ctrl + ,) and navigate to the Add-ons section.
Enable the BlenderKit addon.
Use the search option in the BlenderKit interface to find and import the car model you want by typing "Car" in the search bar.
Click on the car model to import it into your scene.

4. Importing Assets and Applying Them to the Car Model
Open the Asset Browser in Blender.

Drag and drop the desired asset onto the car model where you want the damage texture to be applied.
5. Running the Python Script
After applying the assets, switch to the Scripting workspace.
Python script in the following link:Python Script.
6. Changing the Mode Switcher Node
After running the Python script, go to the Shading tab.

Open the Shader Editor.
Locate the Mode Switcher node in your shader editor.
Add a new Mode Switcher node if it doesn’t appear automatically or change the Mode Switcher to the latest “mode switcher”.
7. Creating Damages
Dents
Adjust the Voronoi Texture and Mapping node scales to create suitable dents on your car model.


Scratches
Modify the values and Mapping node scales to generate appropriate scratches.

Glass Cracks
Add and configure the nodes to simulate realistic glass cracks.


8. Applying dirt texture
To add dirt texture, follow this tutorial Simple Dirt & Dust in Blender - NOT in Substance


9. Applying the HDRI Dome
Instead of importing an HDRI image directly to the world texture,we are using dome hdri.Perks of using dome hdri is it helps in making the car stay on ground unlike world hdri. Follow this tutorial to create the HDRI dome: HDRI Dome Tutorial (Relevant Timeline: 6:03 - 17:38).
You can switch HDRIs by clicking the file icon in the node setup and selecting a different HDRI.

10. Generation
Once you’ve configured everything:
Select the number of samples you want to generate.
Click on Generate to start rendering your car model.

11. Unresolved Challenges
While this guide provides a solid foundation, some challenges remain:
Needs better procedural Dents and scratch texture 
Needs proper lightning to match the background of the car
Dent randomizing on one side
Needs better realism light reflection on car material

Dents need to be implemented manually.
12. Specific Problems that needs to be Addressed 
Needs proper detailing in the hdri environment.
Needs better understanding of geometry nodes for better detailed dents.
No proper placement of dents.


13. Resources
Texture resource: Texture resource
Car models : 	
https://drive.google.com/drive/folders/1pdVvE4Iy5UDwf-opVEpgLbMOX85w-kB3?usp=drive_link
https://sketchfab.com/categories/cars-vehicles
https://free3d.com/3d-models/vehicles
https://www.turbosquid.com/3d-model/free/car

