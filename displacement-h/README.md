![](../images/line3.png)

### Displacement H

<sub>[previous](../first-hour/README.md#user-content-first-hour-in-ue4) • [home](../README.md#user-content-ue4-hello-world) • [next](../readme/README.md#user-content-readmemd-file)</sub>

![](../images/line3.png)

Now that builds a very blocky H.  Now that we have nanite support we can have many more faces and have a fancier font.  How would we take a handwriting font and extrude it with lots of detail?  We can use a displacement map.  Lets do it!

<br>

---


##### `Step 1.`\|`UE5HW`|:small_blue_diamond:

We will be using a displacement map to create a nice font from a plane in UE5.  What is a [displacement map](https://en.wikipedia.org/wiki/Displacement_mapping)? This is a way to use a grayscale map to displace an the points on a model to push them up or down.  Take a look at the video below by clicking on the picture.

[![Watch the video](https://img.youtube.com/vi/1mdR2imNeZI/0.png)](https://youtu.be/1mdR2imNeZI)

![](../images/line2.png)

##### `Step 2.`\|`UE5HW`|:small_blue_diamond: :small_blue_diamond: 

Open up **Photoshop** and create a new file.  Select a **Custom** size.  We want to use a standard texture so we will pick a square resolution with a power of 2 with the most detail we can get.  The more dense the pixels, the greater definition we will have in our displacement map.

The maximum we can use is an 8K texture but what is the exact pixel resolution.  Lets look at the power of 2.  2, 4, 8, 16, 32, 64, 128, 256, 512, 1024, 2048, 4096, 8192.  We want a file that is `8192` square with a **black** background.  Remember that black is no displacement, and white is maximum displacement. We will draw out text in white which will be the extruded letter.

![create an 8192 by 8192 photoshop file with a black background](images/8kTexture.png)

![](../images/line2.png)

##### `Step 3.`\|`UE5HW`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now before I booted up **Photoshop** I installed a font that I wanted to use.  You need to have your font loaded **before** you start photoshop.  I select the **Text** tool and picked the `Vujahday Script` font (from Google Fonts).  The maximum size I can make it is `1296` points but we can scale it more.  Make sure the font color is **PURE** white - `255`, `255` by `255` in the **RGB** channels.

I typed in a capital `H`.

![capital H using vujahday script font](images/pickFont.png)

![](../images/line2.png)

##### `Step 4.`\|`UE5HW`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

While selecting the text layer go to **Edit | Transform | Scale** and scale it up to fill most of the window but giving it some space for an outer glow.  No we cannot have a completely flat extrude we need to have some slope to it.

![scale up H to almost fill screen](images/EditScale.png)

![](../images/line2.png)

##### `Step 5.`\|`UE5HW`| :small_orange_diamond:

So to create a gradation from white to black I have selected a **Layer Style | Outer Glow** and set the **Blend Mode** to `Normal`, the color to `White`, the **Size** to a maximum of `250` px, and added a rounded **Contour**. Please feel free to experiement with your own settings.

![letter H gradation](images/outerGlow.png)

![](../images/line2.png)

##### `Step 6.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond:

Now when you are happy with it we can press **File | Export |Quick Export as PNG**.  Create a new directory in the **Hello World** folder (the same folder that your `.uproject` file is in) and call it `SourceFiles`.  Press the <kbd>Save</kbd> button.

![export H to png and save](images/addedHPNG.png)

![](../images/line2.png)

##### `Step 7.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now in case we want to make tweaks to the **Photoshop** file lets save the source PSD so you can come back to it.  Press **File | Save** and put it in the same **SourceFiles** folder that you used above. Call it `H.psd`.

![save psd to sourcefiles](images/savePSD.png)

![](../images/line2.png)

##### `Step 8.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

![](../images/line2.png)

##### `Step 9.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

![](../images/line2.png)

##### `Step 10.`\|`UE5HW`| :large_blue_diamond:

![alt text](images/.png)

![](../images/line2.png)

##### `Step 11.`\|`UE5HW`| :large_blue_diamond: :small_blue_diamond: 

![alt text](images/.png)

![](../images/line2.png)


##### `Step 12.`\|`UE5HW`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

![alt text](images/.png)

![](../images/line2.png)

##### `Step 13.`\|`UE5HW`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt text](images/.png)

![](../images/line2.png)

##### `Step 14.`\|`UE5HW`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt text](images/.png)

![](../images/line2.png)

##### `Step 15.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond: 

![alt text](images/.png)

![](../images/line2.png)

##### `Step 16.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

![alt text](images/.png)

![](../images/line2.png)

##### `Step 17.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

![](../images/line2.png)

##### `Step 18.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

![](../images/line2.png)

##### `Step 19.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

![](../images/line2.png)

##### `Step 20.`\|`UE5HW`| :large_blue_diamond: :large_blue_diamond:

![alt text](images/.png)

![](../images/line2.png)

##### `Step 21.`\|`UE5HW`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

___

![](../images/line.png)

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - README.md File">

![](../images/line.png)

| [previous](../first-hour/README.md#user-content-first-hour-in-ue4)| [home](../README.md#user-content-ue4-hello-world) | [next](../readme/README.md#user-content-readmemd-file)|
|---|---|---|
