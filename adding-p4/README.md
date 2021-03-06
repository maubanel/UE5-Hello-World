![](../images/line3.png)

### Adding File to Perforce

<sub>[previous](../running-p4/README.md#user-content-running-perforce-in-unreal) • [home](../README.md#user-content-ue4-hello-world) • [next](../project-settings/README.md#user-content-project-settings)</sub>

![](../images/line3.png)

Lets add a new file to the project and submit it to **Perforce**. Lets add a new level to the game that we will start working on and call it **HelloWorld**.

<br>

---


##### `Step 1.`\|`UE5HW`|:small_blue_diamond:

Open up your **Workspace** in **P4V** and open up your project by double left mouse clicking on the `.uproject` to open Unreal.

![open up project](images/doubleClickProject.png)

![](../images/line2.png)

##### `Step 2.`\|`UE5HW`|:small_blue_diamond: :small_blue_diamond: 

 Now make sure that **Source Control** is green.  If not reconnect to source control by signing back in with **Unreal**.

 Press **File | New Level** to load up a new level.

![add a new level](images/doubleCheckSource.png)

![](../images/line2.png)

##### `Step 3.`\|`UE5HW`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now select a new **Empty Level** then press the <kbd>Create</kbd> button.

![create new empty level](images/createEmptyLevel.png)

![](../images/line2.png)

##### `Step 4.`\|`UE5HW`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Open up the **Content Drawer** (you can use the <kbd>Cntrl Space</kbd> as a keyboard shortcut) and right click on **Content** and select `New Folder`.

![add new folder to content ](images/newFolder.png)

![](../images/line2.png)

##### `Step 5.`\|`UE5HW`| :small_orange_diamond:

Call the new folder `Maps`.

![call new folder Maps](images/mapsFolder.png)

![](../images/line2.png)

##### `Step 6.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond:

Now lets save this new level we created.  Press **File | Save Current Level**.

![alt_text](images/fileSave.png)

![](../images/line2.png)

##### `Step 7.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Select the **Maps** folder and name the level.  I named mine `HelloWorld`.  Press the <kbd>Save</kbd> button.

![save level to Maps folder](images/nameFile.png)

![](../images/line2.png)

##### `Step 8.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now right click on your project file and select **Source Control | Check In**.  This will add this file to the **Depot** so other members can **Sync** and see the newly completed level.

![check in new file](images/chekinNewFile.png)

![](../images/line2.png)

##### `Step 9.`\|`UE5HW`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now add an approriate comment to the **Changelist Description**. Make sure the assets are correct, in my case the only thing we are doing is submitting the **Hello World** level to the **Depot**.

Press the <kbd>Submit</kbd> button.

![submit new map to depot](images/addFileToDepot.png)

![](../images/line2.png)

##### `Step 10.`\|`UE5HW`| :large_blue_diamond:

Now you can confirm in **P4V** that this change was pushed to the server.  Select **View | History** and open that tab.  Click on the project ald look at the list of commits.  We can see the one we just created with our comment.

![commit in repo](images/history.png)

![](../images/line2.png)

##### `Step 11.`\|`UE5HW`| :large_blue_diamond: :small_blue_diamond: 

You will also notice that in game the **Red X** is no longer on the file name. This indicates that it is in the **Perforce Depot** now.

![no more red x on this file and it is in the depot](images/noMoreIcon.png)

![](../images/line.png)

![next up setting up the map](images/banner.png)

![](../images/line.png)

| [previous](../running-p4/README.md#user-content-running-perforce-in-unreal)| [home](../README.md#user-content-ue4-hello-world) | [next](../project-settings/README.md#user-content-project-settings)|
|---|---|---|
