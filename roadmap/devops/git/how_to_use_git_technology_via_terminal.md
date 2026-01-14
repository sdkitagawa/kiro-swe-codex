## How to use Git Technology via Terminal

**Translations**

- [EN-US](./how_to_use_git_technology_via_terminal.md)
- [PT-BR](./pt_br/como_usar_a_tecnologia_git_via_terminal.md)

## Navigation
<details>
<summary><b>Menu</b></summary>

- [How to use Git Technology via Terminal](#how-to-use-git-technology-via-terminal)
- [Navigation](#navigation)
- [Setting up your GitHub account](#setting-up-your-github-account)
- [Creating a repository and "downloading" it](#creating-a-repository-and-downloading-it)
- [Navigating through folders using Terminal](#navigating-through-folders-using-terminal)
- [Committing files to GitHub](#committing-files-to-github)
- [Creating directories, moving and renaming files using Terminals](#creating-directories-moving-and-renaming-files-using-terminals)
- [Editing the README file](#editing-the-readme-file)
</details>

## Setting up your GitHub account


- Register to GitHub through the app or the GitHub webpage
- Set up your email (using this command in GitBash)
<br />
<br />

    ```bash
    git config --global user.email "<your email address>"
    ```

## Creating a repository and "downloading" it

- Open your browser and log in to your GitHub account
- Click the "+" sign ➝ Repository ➝ name the repository (try to be logical)  
> #### **Note**: *This is a URL, you can't use space or `'` (single quotation mark), `"` (double quotation marks), `´` (ticks or backticks)*
- Set a description (if you want)
- Set the repository to public
- Turn the Add README option to On
- Add the GNU GPL v3 license (just in case...)
- Create the repository
- Click the green button where it says "code" and copy the repository link (the HTTPS one)
- Go back to the Terminal and navigate to the desired directory (folder)
- "Download" the repository (which is called clone, because it's more than just a simple download), using the code
<br />
<br />

    ```bash
    git clone <your repository link>
    ```
<br />

- Run the list command (`ls`) ➝ find the repository folder ➝ navigate to that folder  
    > #### **Note**: *The "<span style="color: #3A96DD;">(main)</span>" text in blue next to the folder name marks this is the branch you are working on*
<br />

- Get all the files you've been working on, Cut or Copy and Paste them inside that folder you just cloned
    > #### **Note**: *You can do that via Terminal or use Windows Explorer (the common UI or User Interface)*
- Run the list command to check if your files are in the cloned folder
<br />

## Navigating through folders using Terminal

- To navigate to a specific directory

    ```bash
    cd <target directory name>
    ```

    > #### **Note 1**: *You can only go one level at a time*
    > 
    > #### **Note 2**: *This command will only go forwards, not backwards*

- To navigate back to a previous directory or backwards

    ```bash
    cd ../
    ```
    <br />

- To get a list of all the files and directories within a directory

<br />

- **Linux or Windows (WSL, Bash, MSYS)**:

    ```bash
    ls
    ```

- **Windows (Cmd)**:

    ```cmd
    dir
    ```

## Committing files to GitHub

- Uploading the files to your GitHub repository is called a "commit"
- It's called a "commit" because it's a commitment (literally)
- Everything you do here is tracked eternally and there's no way to delete it
- Step one: Run the command (to add all files instead of adding one by one)
    ```bash
    git add .
    ```

- Step two: run the command
    ```bash
    git commit -m "<write a message of your preference, a short description of what you're committing>"
    ```
- Step three: run the command
    ```bash
    `git push origin <the name of the branch you're working on (the blue text next to the name of your  folder)>`
    ```
- Login to your Github account using the browser and authorize  
    > #### **Note**: *Note: You only need to do it once for the device you're using (your laptop or PC)*

- Check the web/app version of the repository on GitHub
- Refresh using F5 on your keyboard  
    > #### **Note**: *It's good practice to keep things organized using folders to separate files into different groups*

## Creating directories, moving and renaming files using Terminals

- To create a new directory (folder)  
    ```bash
    mkdir <directory name>
    ```
- To move files to a directory  
    ```bash
    mv <filename.extension> <target directory name>`
    ```

- Use `ls` in the target directory to make sure you moved the file  
- To rename files or folders  
    ```bash
    mv <old_file_or_folder_name.extension> <new_file_or_folder_name.extension>
    ```

    > #### **Note**: *You will use extensions only for files; use them when naming a file to determine the file type (.txt for Text, .py for Python, .java for Java, etc.)*  
- Run the list command to check the files and file names
    > #### **Note**: *After making changes to your files or folders, make sure to commit those changes to   your GitHub repository*
    > #### **Note**: *Always try to keep your descriptions and file/folder names clear. In Software Engineering, every time you are not being objective and crystal clear, you are telling a lie. And lies are expensive*
- Go to your browser or app and check for the commits  
- Each commit has a code attached to it; everyone can see that; you can't change, delete or remove that

## Editing the README file

- Briefly elaborate on the contents of the repository (what is it about, describe the project briefly)  
- You can add a link for the user reading the README file (To some samples of what you built, the projects you enjoyed the most or the ones that definitely required more of your effort)
- To create links using Markdown:
    ```md
    [Enter word here](Enter link here)
    ```
    > #### **Note**: *make sure the README is in your project folder*

# Credits

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) | [<img src="https://github.com/Romanap4.png?size=50" width=50><br /><sub>@Romanap4</sub>](https://github.com/Romanap4 ) |
| :---: | :---: |
