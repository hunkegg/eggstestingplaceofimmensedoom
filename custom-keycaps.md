# Custom Keycaps
### Ever wanted to spice up your keyboard/Hackpad/fidget toy/where ever you have a keyboard switch?
Try making your own custom keycaps! <br/>
This short guide will go over my process of making **custom keycaps** for my Highway projects (as well as going over some handy CAD commands)

> guide by @egg_splats! check out my other keyboard-related projects, [the Biblically Accurate Keyboard](https://github.com/hunkegg/biblicallyaccuratekeyboard) and [the Engipad](https://github.com/hunkegg/engipad)
> FYI, this guide will be using Fusion 360! 

## ...but why?
Custom keycaps are a nice way to add some personal flair and ***✩ polish ✩*** to your keyboard projects aside from the case and PCB. They can be placed anywhere, such as the escape key on a 75% keyboard or on a macro-binded key on a deskside macropad. <br/>
Custom keycaps can also help with making a **certain theme** more cohesive and "complete", such as the custom keycaps with eyes on my biblically accurate keyboard!
![theming is everything](https://github.com/user-attachments/assets/8b4e52b9-a6bb-40e6-8831-d9e603d32bfa)

## ok how do i start
First, open up your CAD software of choice and create a sketch on the bottom plane. <br/>

Next, you're going to make the bottom face of your keycap. <br/>

Most MX-compatable keycaps use bottom dimensions no bigger than **18mm x 18mm**, so we will be using that as well! Go to the "Create" section of the toolbar and select the Rectangle tool. You can use any of the three rectangle tools, but I personally prefer **Center Rectangle** to keep things centered around the origin. <br/>

Next, draw a rectangle with **18mm x 18mm** dimensions. You can do this while drawing the rectangle by typing in the numbers and using Tab to switch between side dimensions, or use the **Dimensions** tool by clicking D, then clicking on the sides of the drawn rectangle.

![rectangle](https://github.com/user-attachments/assets/15b70d22-7618-4de3-a63d-14bf2951b6fc)

We will also be adding a fillet to the corners of this profile, since a pointy square honestly looks *pretty ugly* <br/>
To do this, click on the **Fillet** tool, then click on two touching sides of the square to make a rounded corner, also called a fillet! I used 2mm as the radius, but the choice is up to you! <br/>

![fillets](https://github.com/user-attachments/assets/a2673334-2ae0-403b-9f2c-3880e932e679)

After you have your base, click "Finish Sketch"! Once we do this, we should have a 18mm x 18mm square sketch with rounded corners. <br/>

![rounded rectangle sketch](https://github.com/user-attachments/assets/ae495a99-a563-4c62-a017-38c8bf9e78a7)

We will be using the **Loft** tool to create the general shape of the keycap. This tool essentially connects two sketch profiles that are on different planes by making a smooth transition between the two profiles. <br/>
![lofty lofty](https://github.com/user-attachments/assets/fb66b0c1-bf00-41c3-b4c7-2ee5e34f3634)
When you look at a regular keycap, you'll typically see the keycap *taper*, or get smaller, near the top. To mimic this shape, we will be using the **Loft** tool alongside a smaller sketch profile to create the shape of the keycap. <br/>

However, to first do this, we need a new plane to make our sketch on! This can be easily done by using the **Offset Plane** Construction tool! As the name implies, this tool makes a new plane to draw sketches on that is *offset*, or extended from, from the original plane. <br/>

To make our new and shiny plane, select the **Offset Plane** tool under Construction and click on the square sketch as our plane. Then, drag the arrow up and down to adjust the height of the plane. <br/>
We will be using 10mm for now! Normal MX keycaps around ~9.75mm, but I'm just rounding here. <br/>
![offset plane](https://github.com/user-attachments/assets/2f4a3711-ddf7-431b-8fe9-30a79e9636ff)
Once we have our plane, select "OK". <br/>

Now that we have our plane, we can make our second sketch required for the Loft! Select the Sketch tool and the newly created plane to create a new sketch on the plane. <br/>
From here, there are many ways to approach making the top profile. Due to the simplicity of the model, we can get away with using a regular old rectangle or circle as our top profile. <br/>
> (I'll get into my own preferred method involving my goat later in the guide :3) <br/>

To make a top profile, draw a circle or rectangle on the sketch plane. The position can vary depending on your preference, but for the sake of the guide, we will be centering the shape on the origin. Set the shape to 15mm on each side or in diameter and click "Finish Sketch".
![2nd profile](https://github.com/user-attachments/assets/b46cbd4f-90b1-4b50-a4b3-c26eddb22465)

Once we do that, we should have two sketch different sketch profiles that look like this:
![ready to loft sir](https://github.com/user-attachments/assets/1c6af4fd-57a5-438b-8fe6-06c63d399c60)

Now, we can use Loft to make our keycap! Select **Loft** under Create, then click on the two sketch profiles. Once we do that, click "OK" to create the body.
![lofty now](https://github.com/user-attachments/assets/b00a443c-d296-4bee-b6f1-a58e3d485c0c)

We now have the general shape of our keycap, but currently, it's COMPLETELY solid. <br/>

However, we can fix that by using the **Shell** Command. 
