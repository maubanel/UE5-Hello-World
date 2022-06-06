![](../images/line3.png)

### Project Settings

<sub>[previous](../adding-p4/README.md#user-content-adding-file-to-perforce) • [home](../README.md#user-content-ue4-hello-world) • [next](../setting-map/README.md#user-content-setting-up-the-map)</sub>

![](../images/line3.png)

Lets now make a change to an existing file in Perforce.  Lets make this new level the one that boots up when we run the editor or the game.

<br>

---


##### `Step 1.`\|`SUU&G`|:small_blue_diamond:

Closwe **UE5** and reopen it.  Does it boot up to the new **Hello World** room?  Look at the tab and see what level is loaded.  It says default!

![defaylt level load](images/defaultLevel.png)

![](../images/line2.png)

##### `Step 2.`\|`FHIU`|:small_blue_diamond: :small_blue_diamond: 

Lets fix it so that the game loads into the level we are working on.  Open up **Edit | Project Settings** and go to **Project | Maps & Modes**. Since this is a one level game and we will only be working on this level lets change the map we boot up to in the editor as well as the one we would start with if we packaged this for a game by changing both **Editor Startup Map** and **Game Default Map** to `HelloWorld`.

![change default startup map](images/changeDefault.png)

![](../images/line2.png)

##### `Step 3.`\|`SUU&G`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now press the <kbd>Source Control</kbd> button at the bottom right and select **Submit Content**.  Then type in an appropriate message and finish by pressing the <kbd>Submit</kbd> button to post it to **Perforce**.

![Commit change to P4](images/commitToP4.png)

![](../images/line2.png)

##### `Step 4.`\|`SUU&G`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

If it succeeded you will see that it submitted a changelist.  Your number will be different than mine.

![GitHub name file LICNESE](images/submitChangelist.png)

![](../images/line2.png)

##### `Step 5.`\|`SUU&G`| :small_orange_diamond:

 Now close **UE5** and reopen it.  You should see that we are now booting up to the **Hello World** room (albeit looks the same all black).

![boot up to hello world map](images/hw.png)


| `ue4.generated.folders`\|`Intermediate & Saved Folders`| 
| :--- |
| *Intermediate - Contains temporary files generated during building the engine or game. In game directories, Shaders are stored in the Intermediate directory.* - [Unreal Docs](https://docs.unrealengine.com/en-us/Engine/Basics/DirectoryStructure)|
|*Saved - Contains autosaves, configuration (.ini) files, and log files. Additionally, the Engine > Saved directory contains crash logs, hardware information, and Swarm options and data.* - [Unreal Docs](https://docs.unrealengine.com/en-us/Engine/Basics/DirectoryStructure)|
|*Intermediate-Contains temporary files generated during building the engine or game. In game directories, Shaders are stored in the Intermediate directory.* - [Unreal Docs](https://docs.unrealengine.com/en-us/Engine/Basics/DirectoryStructure) |


![](../images/line.png)

![next up setting up the map](images/banner.png)

![](../images/line.png)

| [previous](../adding-p4/README.md#user-content-adding-file-to-perforce)| [home](../README.md#user-content-ue4-hello-world) | [next](../setting-map/README.md#user-content-setting-up-the-map)|
|---|---|---|
