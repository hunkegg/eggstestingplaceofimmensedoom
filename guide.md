# Decorative CAD

*Written by @egg_splats on slack* <br/>
[check out my project!!!](https://github.com/hunkegg/biblicallyaccuratekeyboard) <br/>

This is less of a *guide* per se, and more so a collection of CAD techniques used to make the decorative aspects of my previous and Highway projects. <br/>
<img width="300" alt="biblically accurate macropad" src="https://github.com/user-attachments/assets/cb085ad5-4f34-4af0-8f13-1538632a181c" />
<img width="300" alt="toy truck bumper attachment" src="https://github.com/user-attachments/assets/c9f5d41c-9ce6-412b-83b6-dd5bdc61d720" />
<img width="180" alt="shrimp" src="https://github.com/user-attachments/assets/51bec500-ec75-4bdb-b8f4-4decb190dfcb" />

| table o' contents |
| --------- |
| Method 1: Fillets/Chamfer |
| Method 2: Edit Form |
| Methdod 3: Surface Tools |
| general tips! |

## Method 1: Extrude + Fillet/Chamfer
This is by far the simplest way to make something that looks nice. <br/>

I used fillets extensively in my custom keycaps and eye, where I needed to replicate an organic-like shape. Sharp angles are typically not seen in nature, and are often used in more modern/futuristic or man-made designs, such as my toy truck bumper attachment I made for a school assignment. While both can be used interchangably in a simple design, such as making a macropad look a tiny bit better, knowing where to put fillets and chamfers can make a pretty noticable difference.<br/>

<img width="1000" alt="image" src="https://github.com/user-attachments/assets/bdaedd31-52d1-4240-b709-7a50df6b2bc4" /> <br/>

### rounding extrusions!
While fillets are typically used to only round down external edges, the fillet and chamfer command can actually do much more! For example, fillets can round out interior edges, such as the intersection of the bottom and wall of a box. <br/>

<img width="700" alt="image" src="https://github.com/user-attachments/assets/ac676772-4b97-4b78-8fb3-984398323ef5" /> <br/>

Furthermore, the radius of the fillet can extend much further than the height of the wall/floor, allowing for fillets that are "more than 90 degrees" in a sense. <br/>

<img width="700" alt="image" src="https://github.com/user-attachments/assets/504a717b-1322-4ec2-9233-e788d10615c8" /> <br/>

The combination of this technique, as well as some regular fillets are what allowed me to create the unique geometry of the eyes found on the center of my Highway project. The eyelids first started as a regular and boxy extrude, then was blended into the face of the center with an extended fillet, then rounded off by placing more fillets on the remaining sharp corners of the extrude. <br/>

<img width="715" alt="example" src="https://github.com/user-attachments/assets/31aef77f-5f46-48ad-871c-3368543b9fee" /> <br/>

The two fillets on the top of the rectangle led to the top being rounded and circular, while the remaining bottom fillet connected and smoothened everything out into a nice, curvy shape! <br/>

**BUT BE WARNED!!!** The fillet/chamfer tool can also be the source of many headaches and pain! Fusion will typically not allow fillets if a certain part of an extrusion is too small or is destroyed when a fillet is applied! <br/>

<img width="800" alt="I HATE YOU FUSION" src="https://github.com/user-attachments/assets/ec9c4ad6-3ae2-47a4-9473-905e1a8e40a3" />

## Method 2: Create Form
This method is more obscure and difficult than using fillets/chamfers, but can also yeild great results if used correctly! <br/>
<img width="200" alt="image" src="https://github.com/user-attachments/assets/c7a33e14-e5c2-42d2-a0b4-2984179c0f98" />

Create Form is a feature in Fusion 360 that allows users to create objects called "Forms". These forms are different than normal bodies, and are instead made up of faces, edges, and points, as seen in the graphic below. Out of all of these tools, users will most likely be using the **Edit Form** tool, which allows users to move and rotate individual vertices, edges, and faces to morph the form to their liking. <br/>

<img width="1185" alt="image" src="https://github.com/user-attachments/assets/4571d296-b006-40bd-9855-f75ca7971054" /> <br/>

Create form is best used on organic shapes that are often extremely hard to recreate with the standard extrude/loft/sweep of regular CAD.



