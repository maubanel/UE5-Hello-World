<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

### Setting up the Map

<sub>[previous](../ignore-license/README.md#user-content-remaining-github-related-files) • [home](../README.md#user-content-ue4-hello-world) • [next](../setting-sky/README.md#user-content-finish-setting-up-sky)</sub>

<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

Now lets add our **Actor** to our new **Hello World** level.  We will look at a static mesh, textures and a material.  We will also add a light to a scene so we can see the objects.

<br>

---


##### `Step 1.`\|`SUU&G`|:small_blue_diamond:

OK, lets open **UE5**** again through **P4V**.  

![Add three new folders to contents](images/addNewFolder.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`SUU&G`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Go to **Maps & Modes** and change both the **Editor Startup Map** and **Game Default Default Map** to `Test Level`.  Since this is a single level we will be building we can set both to the same.  Normally you would have your first level in the **Game Default** then the level you are currently working on in the **Editor Startup**,
![alt text](images/SetDefaultLevel.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`SUU&G`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

In this exercise you will be spelling out **Hello World**.  So right click on the **TestLevel** in **Content** browser.  Name it `HelloWorld`.

![rename testlevel to helloworld](images/RenameTestLevel.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`SUU&G`| :small_orange_diamond:

Now it is critical that you rename all files and folder **INSIDE** of **UE4**.  Never use the operating system to rename.  If you go back to **Project Settings** you will see that the new level is **Hello World**.  UE4 keeps track of the names so you can rename any object and it will rename all instances of them. Press **File | Save Current** to save your work.

![all files linked look at new name in project settings](images/AllFilesLinked.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`SUU&G`| :small_orange_diamond: :small_blue_diamond:

Now if you saved your work you can see in **GitHub Desktop** what has changed in the game.  Now we will **NOT** use this app to `add` and `commit` these changes.

![files show changes in github desktop](images/FirstChangeInDesktop.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 7.`\|`SUU&G`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Go back to **Unreal** and press the <kbd>Source Control</kbd> button and select **Submit to Source Control**. 

![submit to source control](images/SubmitToSourceControlFirstTime.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 8.`\|`SUU&G`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now you should always include a message in your commits so you know what was done.  **Unreal** forces you to before you can submit the change.  It is a good idea to descrbie what was done a succinctly as possible.

You will see in the bottom right corner a pop up that says the changes have been commited to the **main** branch. Notice that it also saves our commit message.

![commit and submit](images/CommitAndSubmit.jpg)
![commited to main branch](images/CommitedToMainBranch.jpg)


<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 9.`\|`SUU&G`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now this has updated **git** on your local computer.  To make sure it is backed up and on the cloud server you need to **push** this commit (or multiple commits).  I always push when I end a session working in **Unreal** and sometimes throughout the day if it is a long session.  You cannot do this in **Unreal** but have to go back to **GitHub Desktop**.  Notice that it is no longer needing to commit but is one **push** commit behind.  Press the <kbd>Push origin</kdb> button.

![push change to server in github desktop](images/PushUE4ChangeToOrigin.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 10.`\|`SUU&G`| :large_blue_diamond:

For me, errors pop up and I just don't notice them using git.  I always check to make sure that my commit made it to the server.  Go to **GitHub** in your web browser and press on the <kbd>003 commits</kbd>.  Make sure you see your last commit message and if so, it is now safe on the server.

![confirm that git pushed to server](images/CheckPush.jpg)

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Finish Setting Up Sky">

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

| [previous](../ignore-license/README.md#user-content-remaining-github-related-files)| [home](../README.md#user-content-ue4-hello-world) | [next](../setting-sky/README.md#user-content-finish-setting-up-sky)|
|---|---|---|
