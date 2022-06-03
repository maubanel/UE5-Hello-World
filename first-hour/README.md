![](../images/line3.png)

### Installing Unreal & Perforce

<sub>[home](../README.md#user-content-ue4-hello-world) • [next](../setting-up/README.md#user-content-setting-up-unreal--github)</sub>

![](../images/line3.png)

This is a follow up to the introductory Unreal tutorial *Your First Hour in Unreal Engine 5* that will put more of the basics into practice. twist on the usual **Hello World** tutorial which is printing words to a console to introduce someone to a new language.  Since Unreal Engine 5 combines logic, 3-D graphics and a sophisticated editor - this is a multi-disciplinary exercise.  This just introduces creating and importing a 3-D assets, creating a material and material instance and creating logic for a revolving camera. This will give you a start so that you can create your own unique version like the one below.

<p align=center>
<img src="images/loop_01.gif" alt="Animating Hello World in UE4">
</p>
<br>

---

| `required.software`\|`Hello World`| 
| :--- |
| The required software that needs to be downloaded is included below. |

---

##### `Step 1.`\|`FHIU`|:small_blue_diamond:

We will manage all of our games and downloads from a tool that **Epic** provides.  This is used both for playing and making games! Download the **[Epic Game Installer](https://store.epicgames.com/en-US/download)** and install it on your target platform.  I strongly recommend for **Unreal 5** to be using a decent PC (not a mac) with a good separate **AMD** or **NVidia** video card.


![First Hour Tutorial by Unreal](images/installEpicInstaller.png)

![](../images/line2.png)

##### `Step 2.`\|`FHIU`|:small_blue_diamond: :small_blue_diamond: 

Create a free **Epic Game Account**.  If they request licensing, select the **[Standard License](https://www.unrealengine.com/en-US/license)**.  Now run the **Epic Games Launcher** and select the **Settings** option at the bottom left of the interface.


![Epic Games Launcher](images/EpicSettings.jpg)

![](../images/line2.png)

##### `Step 3.`\|`FHIU`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now that you have finished the tutorial, there is one additional piece of information I would like to add.  I prefer to use the native **File Explorer** in both mac & pc's to launch my projects.  This way if I have multiple versions of the same project I know exactly which one I am working on.  Going through their interface abstracts the location and I have seen people save it to a cloud service, or a duplicate version somewhere else on their hard drive.  Navigate to where you have the stored the **Our First Project** folder.  Look for the *.uproject* file with the project name `OurFirstProject`.  If it has the **Unreal** logo you can double click on it and it will load. If you are on a mac this should be setup from default.  In **Windows 10** it often is not setup. If you can load the uproject succesfully you can skip to [step 8](#user-content-step-8fhiu-small_orange_diamond-small_blue_diamond-small_blue_diamond-small_blue_diamond)

![Our first project folder](images/OurFirstProjectFolder.jpg)

If you do not see the Unreal letter in the icon, the PC is not configured to load the project. You need to <kbd>RMB</kbd><kbd>Open With</kbd>. If **UE 4 Editor** shows up select it and go to [step 7](#user-content-step-7fhiu-small_orange_diamond-small_blue_diamond-small_blue_diamond). If not [go to step 4](#user-content-step-4fhiusmall_blue_diamond-small_blue_diamond-small_blue_diamond-small_blue_diamond).

![.uproject not linked](images/UProjectNotLinked.jpg)


<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`FHIU`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Click on the `More Apps` link and we will locate it manually.

![click on more apps](images/MoreApps.jpg)

![](../images/line2.png)

##### `Step 5.`\|`FHIU`| :small_orange_diamond:
 
Scroll to the bottom and select the `Look for another app on this PC` link.

![select look for another app on this pc](images/LookForAnotherApp.jpg)

![](../images/line2.png)

##### `Step 6.`\|`FHIU`| :small_orange_diamond: :small_blue_diamond:

Now locate the folder where you installed this version of Unreal.  By default it will be in `Program Files | Epic Games | UE_4.2X | Engine | Binaries | Win64 | ` and look for the `UE4Editor.exe` and select the <kbd>Open</kbd> button.  This links the Unreal Editor to the`.uproject` file type.  This way when you double click any `.uproject` file it should load it in editor like you want!

![Go to Epic Games Folder and find UE4Editor.exe and select](images/EpicGamesFolder.jpg)

![Uproject has a U icon](images/UE4Editor.jpg)

![](../images/line2.png)

##### `Step 7.`\|`FHIU`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now you should be able to <kbd>RMB</kbd> and select the <kbd>Properties</kbd> button. If you see that it opens with Unreal engine it will work from now on with any new project moving forward!

![Select uproject properties](images/UE4EdtiorInProps.jpg)

![](../images/line2.png)

##### `Step 8.`\|`FHIU`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Lets now go back to the test level.  Go to **Content Browser** and press the <kbd>Filters</kbd> dropdown and select `Level`.  Double click the **TestLevel** (empty level you created in the above walk through with just a floor and atmosphere.

![Reload test level](images/ReloadTestLevel.jpg)

![](../images/line2.png)

##### `Step 9.`\|`FHIU`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now you should see a level that looks like this:

![Reload test level](images/StartingPointTestLevel.jpg)

![](../images/line.png)

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Setting Up Unreal and Github">

![](../images/line.png)

| [home](../README.md#user-content-ue4-hello-world) | [next](../setting-up/README.md#user-content-setting-up-unreal--github)|
|---|---|
