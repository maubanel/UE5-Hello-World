![](../images/line3.png)

### Adding Floor to Level

<sub>[previous](../first-hour/README.md#user-content-first-hour-in-ue4) • [home](../README.md#user-content-ue4-hello-world) • [next](../readme/README.md#user-content-readmemd-file)</sub>

![](../images/line3.png)

Now lets add the floor static mesh we looked at to the level as it is completely empty.

<br>

---


##### `Step 1.`\|`UE5HW`|:small_blue_diamond:

Make sure you booted up the game from **P4V** and that **Source Control** is green.  Make sure you are in the **Hello World** level. Now access the **Content Drawer** (<kbd>Cntrl Space</kbd>) and select the **Static Mesh** folder and drag `SM_Floor` into the level.  Notice everything is black. It did add an instance of the loor to the **Outliner**.

![drag SM_Floor into level](images/DragStaticMesh.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 2.`\|`UE5HW`|:small_blue_diamond: :small_blue_diamond: 

Now the scene is black as there is no sky and no light in the scene.  So the pixels are in the darkness of deep space.  Click on the <kbd>Lit</kbd> button at the top left of the editor game scene and change the lighting mode to **Unlit**.

![switch to unlit mode](images/unlitMode.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`UE5HW`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

So now in the editor we can see the floor but the lighting looks very flat
![unlit mode](images/unlitMode2.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`UE5HW`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now press the green **Play** button and it will be black again.  This **unlit** mode only works in the editor and not in game mode.

https://user-images.githubusercontent.com/5504953/172620693-5a0f5f9e-9879-4601-8b57-373e0dbaaf18.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`UE5HW`| :small_orange_diamond:

Now we need to add a light.  This will be an outdoor scene so lets start with the **Sun**.  This is in game terms a light with no fall off so it runs for infinity.

>The Directional Light simulates light that is being emitted from a source that is infinitely far away. This means that all shadows cast by this light will be parallel, making this the ideal choice for simulating sunlight - [UE5 Manual](https://docs.unrealengine.com/5.0/en-US/directional-lights-in-unreal-engine/)

To find the lights click on the **Place Actors** pull down menu at the top left under the **Tools** menu and select **Light | Directional Light**.

![alt text](images/directionalLight.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond:

Now you can see that there is light.  It might not be positioned properly but we will fix that next.  Now when you hit play you can see the level!  Try it yourself...

![directoinal light in scene](images/addDirectionalLight.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 7.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now there is a special rotational widget that can be used for rotating the light to get different times of day (different angles the sun is position at).  You press the <kbd>Cntrl L</kbd> key to bring up the controller then let go of the <kbd>L</kbd> key while still holding <kbd>Cntrl</kbd>.  You can then move the mouse around and have the sun point at any angle.  I picked one that worked best for me. I then released the <kbd>Cntrl</kbd> key to lock in the position.

https://user-images.githubusercontent.com/5504953/172624138-fdd5d5eb-28ad-4adc-9ada-79f4e447f9e5.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 8.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now we are in a black world - lets create a sky.  Press the **Place Actors** drop down menu and select **Visual Effects | Sky Atmosphere**.

>The Sky Atmosphere component in Unreal Engine is a physically-based sky and atmosphere-rendering technique. It's flexible enough to create an Earth-like atmosphere with time-of-day featuring sunrise and sunset, or to create extraterrestrial atmospheres of an exotic nature. - [UE5 Manual](https://docs.unrealengine.com/5.0/en-US/sky-atmosphere-component-in-unreal-engine/).

Feel free to read the instructions and tweak any values.

![add sky atmosphere to level](images/skyAtmosphere.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 9.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

If it is not working make sure that in your **Directional Light** that 

If you do not see the sky above the black ground plane you can click on the **Directional Light** in the **Outliner** and make sure that **Atmosphere Sun Light** is set to `true`.

![make sure atmosphere sun light in directional light is turned on](images/notWorking.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 10.`\|`UE5HW`| :large_blue_diamond:

Now when you move the **Directional Light** around using <kbd>Cntrl L</kbd> you will see that the color and effect of the sun on the atmposphere changes and you can get sunrise and sunset looks to the lighting in your level.

https://user-images.githubusercontent.com/5504953/172628932-27a4fd2c-9db8-4ccd-8a5e-058882a0f7e5.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 11.`\|`UE5HW`| :large_blue_diamond: :small_blue_diamond: 

In previous versions of Unreal the clouds in the sky was a texture on the skydome, was two dimensional and suffered from the pinching issues of texture mapping a sphere.  Also it had no effect on the light.

In **UE5** we have a more realistic solution with 3-D volumetric clouds.  Select the **Place Actors | VIsual Effects | Volumetric Cloud**

![add volumetric clouds to scene](images/volumetricClouds.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>


##### `Step 12.`\|`UE5HW`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

There is not much to configure here, it is a bit more work to hand craft the clouds to behave in the way you would like.  But feel free to adjust the settings to your taste.

![adjust volumetric cloud settings](images/notConfigurable.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 13.`\|`UE5HW`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

One of the coolest things about 3-D clouds is that it can affect the **Directional Light** and the clouds can cast shadows.  Click on the **Directional Light** and set the **Atmoshpere and Cloud | Casdt Cloud Shadows** to `true`.

https://user-images.githubusercontent.com/5504953/172861626-ffad3d92-ff55-48dd-801d-10125881e425.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 14.`\|`UE5HW`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 15.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond: 

![alt text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 16.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

![alt text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 17.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 18.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 19.`\|`UE5HW`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 20.`\|`UE5HW`| :large_blue_diamond: :large_blue_diamond:

![alt text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 21.`\|`UE5HW`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond:

![alt text](images/.png)

___

![](../images/line.png)

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - README.md File">

![](../images/line.png)

| [previous](../first-hour/README.md#user-content-first-hour-in-ue4)| [home](../README.md#user-content-ue4-hello-world) | [next](../readme/README.md#user-content-readmemd-file)|
|---|---|---|
