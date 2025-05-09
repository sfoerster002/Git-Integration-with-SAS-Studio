
# SAS Studio - Work with a SAS Program from a Git Repository

<br>

## Exercise Description

In this exercise, you will edit a SAS program in your local Git repository and execute it.  Then, review its output and log.  Finally, you will push the changed SAS Program to your fork of the external GitHub repository.

<br>

- [SAS Studio - Work with a SAS Program from a Git Repository](#sas-studio---work-with-a-sas-program-from-a-git-repository)
  - [Exercise Description](#exercise-description)
  - [Execute a SAS Program from your Git Repository](#execute-a-sas-program-from-your-git-repository)
  - [Edit and Re-Execute the SAS Program](#edit-and-re-execute-the-sas-program)
  - [Push the Changed Program to the External Git Repository](#push-the-changed-program-to-the-external-git-repository)
  - [Navigation](#navigation)

## Execute a SAS Program from your Git Repository

1. Open the **Google Chrome** browser on your Windows RACE Image.
1. Select the **SAS Viya** bookmark.
1. Enter the following:
   - User ID: **Alex**
   - Password: **lnxsas**

1. Click **Sign In**.

1. Select ![Viya Menu Selector](images/HamburgerMenu.png) **&#10132; Develop Code and Flows** to open *SAS Studio*.
1. Select ![](images/ExplorerIcon.png) to view the **Explorer** tab in *SAS Studio*.
1. Navigate to **Folder Shortcuts &#10132; Shortcut to MyGitClone** and view its contents.
   
   ![](images/RepositoryContents.png)

2. Double-click the *SAS Program* **TopNCategories.sas** to open the file.
    ![](images/TopNProgram.png)

3. Click ![](images/Run.png) to run the program to create a report for the Top N models by MPG_City for each region of Origin.
   > &#9998; N should be set to 10.
   ![](images/Top10Results.png)

4. Select the **Log** tab to view the log for the executed program.

   ![](images/Top10Log.png)

   > &#9998; There should be no errors or warnings.
5. Select **Notes** to view the notes in the log.
   ![](images/Top10LogNotes.png)

6. Select ![](images/ClearLogIcon.png) to clear the log.
   ![](images/Top10ClearLog.png)

<br>
<br>

## Edit and Re-Execute the SAS Program

1. In the *TopNCategories.sas Code*, change **n** to **5**.

1. Select ![](images/SaveIcon.png) to save the change to the program.
    ![](images/SavedTopN.png)

1. **Run** the program and view its results.
    ![](images/Top5Results.png)

   > &#9998; The results now should be the Top 5 instead of 10.
1. Close the *TopNCategories.sas* program tab.

<br>
<br>

## Push the Changed Program to the External Git Repository

1. Select ![](images/GITIcon.png) to view the **GIT Repositories** tab in *SAS Studio*.
1. Double-click **MyGitClone** to open it in a tab.
   
   ![](images/MyGitUnstaged.png)

   > &#9998; The changed program is listed in the *Unstaged Changes* section.
2. Select the **TopNCategories.sas** in the *Unstaged Changes* section to view the change(s) to the file.
   
   ![](images/FileChanges.png)

3. Select ![](images/StageIcon.png) to stage the selected file.
   
   ![](images/StagedFile.png)

4. Select ![](images/PullMainIcon.png) **&#10132; Pull** to pull any changes that may have happened in the main repository since you cloned it.

   > &#9998; This a good practice to do before you push any changes.

   ![](images/PullMain.png)

5. Enter **Changed N from 10 to 5** for the *commit comment*.

6. Select **Commit** to commit the staged change(s).
   
   ![](images/CommitChanges.png)

7. Select ![](images/PushMainIcon.png) to push the committed changes to the main repository.

8. In *Google Chrome*, navigate to your Github repository to see that the change is reflected there.  You stored the Github link in Visual Studio code in exercise 1.  It should look like this:  **https://github.com/<<(Your Github ID)>>/UsingGitInSASStudio**.

9.  Click **Sign in** to sign in with your *GitHub* credentials.

10. The **TopNCategories.sas** file should have your commit comment listed.


   ![](images/UpdatedFork.png)

<br>
<br>

## Navigation

<!-- startnav -->
* [01 SAS Studio-Git-Integration-Setup](/01_SAS-Studio-Git-Integration-Setup.md)
* [02 SAS Studio SAS Program](/02_SAS_Studio_SAS_Program.md)**<-- you are here**
* [03 SAS Studio GIT Branches 1](/03_SAS_Studio_GIT_Branches_1.md)
* [04 SAS Studio GIT Branches 2](/04_SAS_Studio_GIT_Branches_2.md)
<!-- endnav -->
