# Appdev Reviewer — GitHub to VS Code Live Server

Follow these steps to download the reviewer to your computer and run it in your browser using VS Code.

## 1. Install Visual Studio Code

1. Open the [official VS Code download page](https://code.visualstudio.com/download).
2. Download the installer for your operating system.
3. Run the installer and finish the installation.
4. Open **Visual Studio Code**.

## 2. Download the project from GitHub

Choose **one** of the following methods, then continue to Step 3.

### Method A: Download ZIP — no Git installation needed

1. Open the [AppDev-Reviewer repository](https://github.com/maki-sushi-distro/AppDev-Reviewer) in your browser.
2. On the repository's main page, click the green **Code** button.
3. Select **Download ZIP** and wait for the download to finish.
4. Open your computer's **Downloads** folder.
5. On Windows, right-click the ZIP and choose **Extract All…**, then **Extract**. On macOS, double-click the ZIP to extract it.
6. Open the extracted folder and locate **appdev-reviewer.html** and **code-questions.json**.

Keep both files together. Run the extracted files, not the files inside the ZIP. The extracted folder name may include the branch name, such as `AppDev-Reviewer-main`.

Git and terminal commands are not required for this download method. See [GitHub's archive download instructions](https://docs.github.com/en/repositories/working-with-files/using-files/downloading-source-code-archives) for more detail.

### Method B: Git Clone

1. If Git is not installed, download it from the [official Git website](https://git-scm.com/downloads) and finish the installation.
2. Open a new terminal: **PowerShell** on Windows or **Terminal** on macOS/Linux.
3. Check that Git is available:

   ```bash
   git --version
   ```

4. Navigate to the folder where you want to save the project. For example, use your Downloads folder:

   ```bash
   cd ~/Downloads
   ```

5. Clone the repository:

   ```bash
   git clone https://github.com/maki-sushi-distro/AppDev-Reviewer.git
   ```

6. Enter the newly created project folder:

   ```bash
   cd AppDev-Reviewer
   ```

7. Continue to Step 3 and open this **AppDev-Reviewer** folder in VS Code. No ZIP extraction is needed for this method.

If `git` is not recognized after installation, close and reopen your terminal, then try `git --version` again.

## 3. Open the project folder in VS Code

1. In VS Code, select **File → Open Folder…**.
2. Browse to the extracted folder from Method A or the cloned **AppDev-Reviewer** folder from Method B.
3. Select the folder that directly contains **appdev-reviewer.html** and **code-questions.json**, then click **Select Folder** or **Open**.
4. Confirm that both filenames appear in VS Code's **Explorer** on the left.

## 4. Install the Live Server extension

1. Open **Extensions** from the left sidebar, or press **Ctrl + Shift + X** on Windows/Linux (**Cmd + Shift + X** on macOS).
2. Search for **Live Server**.
3. Select **Live Server** by **Ritwick Dey**, extension ID `ritwickdey.LiveServer`.
4. Click **Install**. If it is already installed, make sure it is enabled.
5. Return to the **Explorer** panel.

You can confirm the extension on its [official Marketplace page](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer).

## 5. Start the reviewer

1. In VS Code's Explorer, right-click **appdev-reviewer.html**.
2. Click **Open with Live Server**.
3. Your browser opens the reviewer. The question bank loads automatically from **code-questions.json**.
4. Start with **Study Notes**, **Write-the-Code**, **Identification**, or **Mock Exam**.

The address will normally resemble:

```text
http://127.0.0.1:5500/appdev-reviewer.html
```

Use the address Live Server opens; the port may differ. If a folder listing opens, click **appdev-reviewer.html**. Keep VS Code and Live Server running while using the app.

No `npm install`, Node.js, Python, database, or separate backend is required. After downloading the project and installing VS Code/Live Server, the reviewer works without internet access.

## 6. Stop or reopen the reviewer

- To stop: open VS Code's Command Palette with **Ctrl + Shift + P** (**Cmd + Shift + P** on macOS), then run **Live Server: Stop Live Server**.
- To reopen later: open the same project folder and repeat Step 5.
- To use an updated version: download and extract it into a new folder, keeping its HTML and JSON together, then open that folder in VS Code and repeat Step 5.

## Troubleshooting

| Problem | What to do |
|---|---|
| **Open with Live Server** is missing | Check that Live Server is installed and enabled, open the project as a folder, and right-click the `.html` file. |
| The browser says the site cannot be reached | Start Live Server again and use the address it opens. |
| A folder listing appears | Click **appdev-reviewer.html**. |
| The app asks you to choose a JSON file | A `file://` address means you opened the HTML directly; use **Open with Live Server** for automatic loading. |
| The questions fail to load | Check that **code-questions.json** is beside **appdev-reviewer.html**, then select **Retry loading**. |
| Old questions or content appear | Refresh the browser; on Windows, try **Ctrl + F5**. Check that Live Server is serving your updated folder. |

Progress exists only while the page stays open. Refreshing or closing it clears answers and results. The optional mock-exam countdown pauses in Study Notes and resumes when you leave.
