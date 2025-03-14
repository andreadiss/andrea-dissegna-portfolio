Initial Setup (First-Time Users)
If you haven’t cloned the repository to your local machine yet, follow these steps:
Open a Terminal:
On Windows: Open Git Bash or Command Prompt.

On macOS/Linux: Open Terminal.

Navigate to Your Working Directory:
bash

cd C:\Users\andre

Clone the Repository:
bash

git clone https://github.com/andreadiss/andrea-dissegna-portfolio.git

This creates the folder C:\Users\andre\andrea-dissegna-portfolio.

Navigate to the Project Directory:
bash

cd andrea-dissegna-portfolio

Verify the Files:
Ensure the directory contains index.html, the images/ folder, and any media files (e.g., journey_map.png, bar_chart.png, Media1.gif).

Making Amendments to the Local index.html File
Step 1: Open the index.html File
Navigate to C:\Users\andre\andrea-dissegna-portfolio in File Explorer (Windows) or Finder (macOS).

Right-click index.html and open it with your preferred text editor (e.g., Visual Studio Code).

Step 2: Make Changes
Edit Text: Modify the content directly in index.html. For example, update project descriptions or section titles.

Add or Replace Media:
To add a new image or GIF, place the file in the images/ folder (e.g., C:\Users\andre\andrea-dissegna-portfolio\images).

Reference the new file in index.html using a relative path. Example:
html

<div class="image-placeholder">
  <img src="images/new_image.png" alt="Description of the image">
  <p class="caption">Caption for the new image</p>
</div>

To resize an image (e.g., to 1/4 size), add the resized class:
html

<img src="images/new_image.png" alt="Description of the image" class="resized">

Ensure the file path matches the file name exactly (case-sensitive).

Step 3: Save Changes
After editing, save the index.html file in your text editor.

Step 4: Test Locally (Optional)
Double-click index.html to open it in your default web browser and verify your changes (e.g., check if images/GIFs load correctly).

If media doesn’t load, ensure the file is in the images/ folder and the path in index.html is correct.

Adding Changes to GitHub
Step 1: Navigate to the Project Directory
Open a terminal (Git Bash, Command Prompt, or Terminal).

Navigate to the project directory:
bash

cd C:\Users\andre\andrea-dissegna-portfolio

Step 2: Stage the Changes
Add Modified Files:
To stage the updated index.html:
bash

git add index.html

If you added new media files (e.g., new_image.png), stage them as well:
bash

git add images/new_image.png

To stage all changes at once (including new files):
bash

git add .

Verify Staged Files:
Check the status of your changes:
bash

git status

You should see the modified files (e.g., index.html, images/new_image.png) listed under "Changes to be committed."

Step 3: Commit the Changes
Commit your changes with a descriptive message:
bash

git commit -m "Update index.html with new image and text changes"

Replace the message with something specific to your changes, e.g., "Add new_image.png to Project 2" or "Update project description in index.html".

Step 4: Push to GitHub
Push the committed changes to the main branch on GitHub:
bash

git push origin main

If prompted, enter your GitHub username and password (or use a personal access token if required).

