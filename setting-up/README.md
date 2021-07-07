<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

### Setting Up Unreal & Github

<sub>[previous](../first-hour/README.md#user-content-first-hour-in-ue4) • [home](../README.md#user-content-ue4-hello-world) • [next](#)</sub>

<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

Before we can start we want to set up our development environment. This includes setting up **GitHub** as our version control so we can backup and maintain our project safely. Make sure you have lots of hard drive space as the engine and various downloads can take a lot of room. I recommend around 100 gigabytes free would be suitable.

<br>

---

| `important.concept`\|`Version Control`| 
| :--- |
| There are some potential problems developing with a complex engine:<br>
:small_blue_diamond: The engine can crash and you can lose your work<br>
:small_blue_diamond: You can forget the data on another computer<br>
:small_blue_diamond: Your hard drive can die and all the data can be lost<br>
All of these problems can be avoided if we use **version control** to back up our data.  This way we can recover lost work, *clone* the data on another computer and collaborate as a team.  It is a good idea to get used to using version control as all large projects use them. The good news is that you have the tools integrated right in Unreal. |

---

##### `Step 1.`\|`SUU&G`|:small_blue_diamond:

If you are on a mac git comes ready to go (it might need to install xcode when first running the command).  On a PC you will need to install [git](https://git-scm.com/downloads).  Double click and keep all the default suggestions.  Follow the directions on the website for installing it on PC.

![screenshot from git website download page](images/GitForPC.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 2.`\|`FHIU`|:small_blue_diamond: :small_blue_diamond: 

Now so you don't have to use command line prompts for git it is a good idea to install a GUI and the one I like best is [Github Desktop](https://desktop.github.com) as it integrates with GitHub perfectly.  Download and install the software.

![GitHub desktop download webpage](images/GitHubDesktop.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`SUU&G`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now since game projects can get very large and graphics, and 3-D models can take a lot of space it is best to use the [Git LFSn (Large File System)](https://git-lfs.github.com) extension for games.  This way only assets that are currently being used are downloaded to your system speeding up your workflow and allowing you to hold larger files in GitHub. Install it on your computers per the directions on the website.

![GitHub LFS webpage](images/GithubLFS.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`SUU&G`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

In the editor select the **Edit** menu item then from the drop down menu select **Editor Preferences**. Select **Loading & Saving** tab from the left hand side.  Go to *Source Control* and set **Prompt for Checkout on Asset Modification** to `true` and **Add New Files when Modified** to `true`.  Leave the other two settings at `false` and accept their default editor to deal with merge conflicts. 

https://user-images.githubusercontent.com/5504953/124603352-b3b06880-de1e-11eb-926e-a913b741c38b.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`SUU&G`| :small_orange_diamond:

Make sure you have a **GitHub** account and that you are logged into it.  Click on [GitHub Classroom Hello World Link](https://classroom.github.com/a/z7lsXBo4).  Accept the prompt if it asks you go join the class and you should get to a **Accept the Assignment – UE4-Hello-World-FA21**.  Press the <kbd>Accept this assignment</kbd> button.

![Accept GitHub Classroom Assignment](images/AcceptThisAssignment.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`SUU&G`| :small_orange_diamond: :small_blue_diamond:

You will get a message saying the repository is geing setup.  Refresh/Reload your web browser as instructed.

![refresh web browser](images/RefreshBrowser.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 7.`\|`SUU&G`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Eventually you will get a link for the repository.  Click on this link:

![link to new repository for assignment](images/NewHelloWorldRepository.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 8.`\|`SUU&G`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now our server has no files on it. We will be using command line (**Terminal** on the mac Or **Git Bash** on the PC). You can see the commands below.  We are creating a **main** branch and making it our default branch (`-M` switch).  We are then taking the content we **Already Have** in our folder and pushing it to the server.

![empty github repository](images/PushToExistingRepository.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 9.`\|`SUU&G`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Lets start by copying the link to the clipboard so we can add it to Unreal, and use UE4 to **Initialze** the project.

![Copy repository link](images/CopyRepositoryLink.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 10.`\|`SUU&G`| :large_blue_diamond:

Go back to **Unreal Engine** and press the <kbd>Source Control</kbd> button and select the **Provider** `None` dropdown.

![select github for source control](images/SelectGitHubForSourceControl.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 11.`\|`SUU&G`| :large_blue_diamond: :small_blue_diamond: 

In the menu select **Git (beta version)** as the source control you will be using. Paste the directory for your GitHub project into the **Url of the remote server 'origin'** in Unreal.  Then make sure you add a **.gitignore** file, a **README.md** file, a **.gitattributes for Git LFS** file and finally **Make the initial Git Commit** file.  Then press the **Intialize project with Git** button and on the next pop up press the **Accept Settings** button. You should see message pop up saying *Connection to source control was successful!*.

![setup github repository](images/SetupGitRepo.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>


##### `Step 12.`\|`SUU&G`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

Lets make sure it installed GitHub in our project.  First we need to turn on hidden folders. On the PC follow these [Windows 10 Turn on Hidden Folders](https://support.microsoft.com/en-us/help/4028316/windows-view-hidden-files-and-folders-in-windows-10) directions. On the Mac it is a bit more involved so go and [turn on hidden folders on Mac](https://ianlunn.co.uk/articles/quickly-showhide-hidden-files-mac-os-x-mavericks). You should now see a `.git` hidden folder in the root directory of the project, if you do – you succesfully created a GitHub repo and connected it to the server.

![turn on hidden folders](images/HiddenFolders.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 13.`\|`SUU&G`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

Now we are going to use the **Command Line** tools just once.  On a **PC** run **Git Bash

![turn on hidden folders and confirm .git](images/ConfirmDotGitLoder.jpg)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>




<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - ???">

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

| [previous](../first-hour/README.md#user-content-first-hour-in-ue4)| [home](../README.md#user-content-ue4-hello-world) | [next](#)|
|---|---|---|
