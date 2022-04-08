# ENGL 1102 Artifact 3: Digital Game
Authors: Ammar Deafalla, Emily Zhao, Hunter Rewis, Mckenna Taylor, Sean Jmaes

## TODO

## GAMEPLAY LOOP INFO

## HOW TO SET UP ON LOCAL MACHINE

### SETTING UP GIT
1. Make sure you have Git installed
	- If you're on Linux, this is easy - use your package manager
    - If you're on Windows or Mac, download GitHub Desktop from [here](https://desktop.github.com)
2. Ensure Git or GitHub Desktop is configured
    - With GitHub desktop, it should just be as easy as logging into it
    - With Git, if you haven't configured it, you will have to run `git config --global user.name <your GitHub username>` and `git config --global user.email <your GitHub email>`

### WORKING WITH THE BROWSER APP
1. Pick a folder to store the Git repository in. It can be anywhere you like
2. Clone the GitHub repository into whatever folder you chose
    - On GitHub Desktop: select the repository from the list and use the "Choose" option for the path to save it to the folder you chose
    - Using Git on the command line: from the "Twine" folder, run `git clone <path to repo> <your folder name>`
        - **SPECIAL NOTE:** If using Git from the command line, you will have to have an SSH key set up and added to your GitHub account because you can only use SSH to clone from GitHub via the command line if the repository is private
3. Congratulations, you're all set up! Working with the browser app is a bit more complicated than the desktop app, though
    - To start working:
        1. Use GitHub Desktop (or the appropriate `git` commands) to pull/sync with the remote GitHub repository
        2. Open the Twine website and import the latest published story/Twine archive
        3. Replace whatever story you have saved with the version you're importing (unless you need both versions)
    - To sync your progress OR when you stop working:
        1. Go to the home page
        2. Publish the story OR save an archive (be sure to save the file!)
        3. Move that file to the folder the Git repository is in
        4. Use GitHub Desktop (or the appropriate `git` commands) to commit and push your changes
    - **Working with published story files is preferred since the naming scheme stays consistent**


### WORKING WITH THE DESKTOP APP
1. Download the Twine desktop app [here](https://twinery.org/). Once you've downloaded and installed (Win & Mac)/unzipped (Linux) the file, open the app and go through the little setup
    - You will have to tell Windows Defender to allow the download of the app, and to allow it to run. If you don't want to deal with this and are a bit savvy with Node.js and npm, visit [this GitHub repository](https://github.com/klembot/twinejs) for instructions (you might still have to deal with Windows Defender, I didn't try this method)
2. Find where Twine stores the stories. It should be under "Documents/Twine/Stories". If not, contact Stephen
3. Delete the "Stories" folder
4. Clone the GitHub repository into "Twine/Stories"
    - On GitHub Desktop: select the repository from the list and use the "Choose" option for the path to save it to "Twine/Stories"
    - Using Git on the command line: from the "Twine" folder, run `git clone <path to repo> Stories/`
        - **SPECIAL NOTE:** If using Git from the command line, you will have to have an SSH key set up and added to your GitHub account because you can only use SSH to clone from GitHub via the command line if the repository is private
5. Congrats, you're all set up!
    - To start working:
        1. Use GitHub Desktop (or the appropriate `git` commands) to pull/sync with the remote GitHub repository
        2. Open the Twine website and import the latest published story/Twine archive
        3. Replace whatever story you have saved with the version you're importing (unless you need both versions)
    - To sync your progress OR when you stop working:
        1. Use GitHub Desktop (or the appropriate `git` commands) to commit and push your changes

## WORKFLOW
We will be using the "[GitFlow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)" workflow to manage workflow.
- The "main"/"master" branch will be for "major" versions of the story
- The "dev" branch will be used for versions of the story that we aren't quite ready to release yet
- Individual "feature" branches (with names that change accordingly) will be used for working on specific parts of the story
    - For example, one story path could be worked on in one branch, while another path is worked on in another

### DEALING WITH MERGE CONFLICTS
The easiest way to deal with merge conflicts is to **make sure we communicate about who is working on what**.
If a merge conflict comes up, we all have to agree on what to keep and what to remove. Only then can the conflict be resolved.

### HOW TO ADD PASSAGES PROGRAMATICALLY
[Undocumented feature](https://github.com/tmedwards/sugarcube-2/blob/master/src/story.js#L357] in (SugarCube API)[http://www.motoslave.net/sugarcube/2/docs/#story-api).
