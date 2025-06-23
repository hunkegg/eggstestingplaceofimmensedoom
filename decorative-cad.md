# Decorative CAD

*Written by @egg_splats on slack* <br/>
[check out my project!!!](https://github.com/hunkegg/biblicallyaccuratekeyboard) <br/>

This is less of a *guide* per se, and more so a collection of CAD techniques used to make the decorative aspects of my previous and Highway projects. <br/>
![Screenshot 2025-06-23 at 2 50 52 PM](https://github.com/user-attachments/assets/3ecc2969-7dde-441b-b96a-2384d495cf95)
> this guide will sadly only go over Fusion, but onshape usually has lots of features similar to those mentioned in this guide!

| table o' contents |
| --------- |
| general tips! |
| Method 1: Fillets/Chamfer |
| Method 2: Edit Form |
| Methdod 3: Surface Tools |

## General Tips!
I mainly want to get these out of the way first, since they can be applied to nearly anything in CAD, whether decorational or not! <br/>

### 1) Construct tools are GOATED
The Contstruct Tools in Fusion are a set of tools that allow the user to create objects to base sketches or commands off of. While they may seem useless at first, they can be extremely helpful in making more custom and cooler designs! <br/>
![construct tool list](https://github.com/user-attachments/assets/5f47445c-deca-4dc2-beda-61772ab794d3)

For example, in my Highway project, I could've copy and pasted a keyswitch section 8 times and moved them around to form a ring, but I instead used the Construct tool **"Axis Perpendicular to a Face at Point"** in combination with a sketch to create an axis of rotation to use a Circular Pattern. (i know that sounds like jargon but i'll try my best to break it down) <br/>

Essentially, the Circular Pattern tool allows me to copy a part in Fusion around in a circle, and requires an axis to rotate around. First, I drew a sketch on the part to find the "center" of the ring, then created an axis through that point with the Construct tool. Since that axis is exactly in the center of the ring, I can use that axis for my Circular Pattern, making the process **MUCH** easier and faster.
![axis tool example](https://github.com/user-attachments/assets/91520ea6-e8fa-424f-ad18-5cee93b7e016)

Construct tools often feed or help with other tools, such as **Offset Plane** or **Plane at Angle** helping with *custom angles in sketches*, or the **Axis** tools helping with Pattern-type tools like *Rectangular/Circular Pattern* as mentioned above. I ***strongly*** recommend learning these if you want to improve your modeling! <br/>
> offset plane is my favorite btw, super good for the loft tool!

### 2) Learn more Fusion tools!
While *Extrude* may get you by 80% of the time in CAD, learning other tools can help spice up your design! I ***strongly*** recommend getting familiar with the 4 tools mentioned below! <br/>
![the fantastic fusion four](https://github.com/user-attachments/assets/0cda8f34-e9cb-4c1a-b3e2-ce0fe9ef4ddf)
| tool name | purpose |

| --------- | --------- |
| extrude | the basic extrude; extends a sketch perpendicular to the sketch plane |
| revolve | revolves a sketch around an axis; good for objects like vases or bottles |
| sweep | extends a sketch along a custom path (often another sketch perpendicular to the other sketch plane); good for pipes or tubes |
| loft | connects the edges between two sketches; good for adapters or in my case, keycaps! | <br/>
![loft example on keycap](https://github.com/user-attachments/assets/5e933a2d-cbf5-46ac-bc67-debc4148f7db)
> an example of loft in action! I used **Offset Plane** to create the other sketch, then used loft to create the general shape of the keycap

Here is a list of other Fusion tools I recommend learning:
| tool name | purpose | location |
| --------- | --------- | --------- |
| Project | used in sketches, projects a 3D object onto a sketch plane. ***VERY*** helpful in designing screw holes for PCBs or for making correct sizings for other parts like keycap stems. | Sketch Tab (shows up when making a sketch) > Create Tools > Project/Include > Project (keybind should be **P** by default) |
| New Component | used to store components in CAD. helpful for organizing models with a million imported components like my keyboard. | Solid Tab > Assemble > New Component |
| Appearance | used to add materials and colors to bodies in your model. helpful for visualizing the final result, as well as making the CAD pictures for submission look pretty :D | Solid Tab > Modify > Appearance (keybind should be **A** by default) |
| Constraints | used in sketches, constrains certain elements like lines or points into a "relationship" (equal length (equal), at the same point (coincident), perfectly horizontal/vertical, etc.). **Very** helpful for designing geometric or precise sketches like the mount and casing of a PCB. | Sketch Tab > Constraints (symbols with red lines!) |
| Canvas | used to add a picture on a surface as reference for modeling. ***VERY*** helpful for designing decoration, such as the eyes on my keycaps/center, since you can just trace the canvas without issue. | Solid Tab > Insert > Canvas |
> note: "Tab" refers to the sections right above the tool icons (Solid, Surface, Mesh, Sheet Metal, Plastic, Utilities, Manage)
![canvas tool example](https://github.com/user-attachments/assets/e84e7454-25c5-4d56-83fb-854b5efe058d)
> examples of using the Canvas tool to design the decorative eyes!

## Method 1: Fillet/Chamfer
This is by far the simplest way to make something that looks nice. <br/>

I used fillets extensively in my custom keycaps and eye, where I needed to replicate an organic-like shape. Sharp angles are typically not seen in nature, and are often used in more modern/futuristic or man-made designs, such as my toy truck bumper attachment I made for a school assignment. While both can be used interchangably in a simple design, such as making a macropad look a tiny bit better, knowing where to put fillets and chamfers can make a pretty noticable difference.<br/>

![sugarcoat](https://github.com/user-attachments/assets/174e4518-ddf9-41ae-bbdc-9f40f0dac32b)

### rounding extrusions!
While fillets are typically used to only round down external edges, the fillet and chamfer command can actually do much more! For example, fillets can round out interior edges, such as the intersection of the bottom and wall of a box. <br/>

<img width="868" alt="rounding 1" src="https://github.com/user-attachments/assets/5711001c-e7d3-4232-95ad-a6f613d1c604" />

Furthermore, the radius of the fillet can extend much further than the height of the wall/floor, allowing for fillets that are "more than 90 degrees" in a sense. <br/>

<img width="919" alt="rounding 2" src="https://github.com/user-attachments/assets/860b3b99-2650-4f1c-a55d-be7bdf108d1a" />

The combination of this technique, as well as some regular fillets are what allowed me to create the unique geometry of the eyes found on the center of my Highway project. The eyelids first started as a regular and boxy extrude, then was blended into the face of the center with an extended fillet, then rounded off by placing more fillets on the remaining sharp corners of the extrude. <br/>

![rounding example](https://github.com/user-attachments/assets/08e4f26c-eca8-41ad-868d-eee5a3a92f4e)

The two fillets on the top of the rectangle led to the top being rounded and circular, while the remaining bottom fillet connected and smoothened everything out into a nice, curvy shape! <br/>

**BUT BE WARNED!!!** The fillet/chamfer tool can also be the source of many headaches and pain! Fusion will typically not allow fillets if a certain part of an extrusion is too small or is destroyed when a fillet is applied! <br/>

![I HATE YOU FILLETS](https://github.com/user-attachments/assets/06ed14f7-4f9d-40eb-bf36-6aa09761b6a7)

## Method 2: Create Form
This method is more obscure and difficult than using fillets/chamfers, but can also yeild great results if used correctly! <br/>

![create form](https://github.com/user-attachments/assets/7e67bd24-d7a0-436a-acc4-0c4ca0786b52)

**Create Form** is a feature in Fusion 360 that allows users to create objects called **"Forms"**. These forms are different than normal bodies, and are instead made up of faces, edges, and points, as seen in the graphic below. Create Form offers a new set of tool, but users will most likely be using the **Edit Form** tool, which allows users to move and rotate individual vertices, edges, and faces to morph the form to their liking. <br/>

![forms](https://github.com/user-attachments/assets/854d225d-90da-4bf7-b698-62d953948541)

Create form is best used on **organic or irregular shapes** that are often extremely hard to recreate with the standard extrude/loft/sweep of regular CAD. For example, I used Create Form to make a seat as part of a chair project for school, which allowed me to make a unique and comfortable shape for the seat. <br/>

The use of Create Form also allowed me to *easily change the geometry* of the seat with the Edit Form tool. While regular extrusions require going back to the sketch and changing dimensions, Forms can be directly morphed by dragging and rotating vertices and lines, making Forms much easier to work with when dealing with complex, irregular shapes. <br/>
> btw for those curious, the seat was made out of a Form cube with two of the main faces removed, then was morphed around with Edit Form to resemble a chair. <br/>

![chair example](https://github.com/user-attachments/assets/ace4240a-bc54-49e0-9592-be7a6b8df8a7)

**However, Edit Form isn't limited to just complex shapes!** You can easily get away with spamming simple shapes if your design needs it, such as in the case of my shrimp chef. <br/>
In this example, I used Edit Form to repeatedly place spheres to create the eyes and chef hat! While this may seem inefficient at first, making each of these spheres individually with the Revolve command would take much, ***much*** longer! <br/>

![shrimp example](https://github.com/user-attachments/assets/1acf91c9-2e85-4e8e-9786-394be7285a44)





