# Exercise: Building and Version Controlling a Personal Portfolio Website

**Objective**: Learn how to create a simple personal portfolio website using HTML and CSS and manage the project using Git for version control.

**Prerequisites**:
- Basic understanding of HTML and CSS.
- Basic knowledge of Git and GitHub.
- Git installed on your computer.
- A GitHub account.

## Instructions

### Step 1: Create a Repository on GitHub

1. **Create a New Repository**:
   - Go to [GitHub](https://github.com) and log into your account.
   - Go to our [collab team github](https://github.com/orgs/collabexpress/repositories)
   - Click on the **New Repository** button to create a new repository.
   - Name your repository `<<name>>-portfolio` e.g. jane-portfolio.
   - Add a description if you like (optional).
   - Make repository as **Public** .
   - **Do not** initialize the repository with a README, .gitignore, or a license (you will do this locally).
   - Click **Create repository**.

2. **Copy the Repository URL**:
   - Once the repository is created, you will be redirected to the repository page.
   - Copy the URL of your new repository (it should look something like `https://github.com/<<teamname>>/<<name>>-exercise1.git`).

### Step 2: Set Up Your Project Locally

1. **Create a New Directory**:
   - Open your terminal (Command Prompt, PowerShell, or Git Bash).
   - Navigate to the location where you want to create your project folder.
   - Create a new directory named `<<name>>-portfolio` and navigate into it:
     ```sh
     mkdir <<name>>-portfolio
     cd <<name>>-portfolio
     ```

2. **Open the project via VS Code**:
    - via terminal:
    ```sh
     cd <<name>>-portfolio
     code .
     ```
    or
    - via vs code

3. **Initialize Git Repository**:
   - Initialize a new Git repository in your project directory:
     ```sh
     git init
     ```

4. **Add Remote Repository**:
   - Link your local repository to the GitHub repository you just created:
     ```sh
     git remote add origin https://github.com/<<teamname>>/<<name>>-exercise1.git
     ```

5. **Create Initial Files on the project**:
   - index.html
   - styles.css

### Step 3: Create the HTML Structure

1. **Edit `index.html`**:
   - Open `index.html` and add the basic HTML structure:
     ```html
     <!DOCTYPE html>
     <html lang="en">
     <head>
         <meta charset="UTF-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
         <title>My Portfolio</title>
         <link rel="stylesheet" href="styles.css">
     </head>
     <body>
         <header>
             <h1>Welcome to My Portfolio</h1>
         </header>
         <main>
             <section id="about">
                 <h2>About Me</h2>
                 <p>This is a brief introduction about myself.</p>
             </section>
             <section id="projects">
                 <h2>Projects</h2>
                 <p>Here are some of my projects.</p>
             </section>
         </main>
         <footer>
             <p>&copy; 2024 My Portfolio</p>
         </footer>
     </body>
     </html>
     ```

2. **Commit Your Changes**:
   - Save your changes and commit them:
     ```sh
     git add index.html
     git commit -m "Initial commit with basic HTML structure"
     ```

### Step 4: Style Your Website with CSS

1. **Edit `styles.css`**:
   - Open `styles.css` and add basic styling:
     ```css
     body {
         font-family: Arial, sans-serif;
         margin: 0;
         padding: 0;
         background-color: #f4f4f4;
     }

     header {
         background-color: #333;
         color: white;
         padding: 1em;
         text-align: center;
     }

     main {
         padding: 1em;
     }

     section {
         margin-bottom: 2em;
     }

     footer {
         background-color: #333;
         color: white;
         text-align: center;
         padding: 1em;
         position: fixed;
         width: 100%;
         bottom: 0;
     }
     ```

2. **Commit Your Changes**:
   - Save your changes and commit them:
     ```sh
     git add styles.css
     git commit -m "Add basic styling"
     ```

### Step 5: Create a New Branch

1. **Create and Switch to a New Branch**:
   - Create a new branch named `feature/exercise-1` and switch to it:
     ```sh
     git checkout -b feature/exercise-1
     ```

2. **Add New Content**:
   - In `index.html`, add a new section under the existing sections:
     ```html
     <section id="contact">
         <h2>Contact Me</h2>
         <p>Email: your-email@example.com</p>
     </section>
     ```

3. **Commit Your Changes**:
   - Save your changes and commit them to the new branch:
     ```sh
     git add index.html
     git commit -m "Add contact section"
     ```

### Step 6: Merge the Branch into the Master Branch

1. **Switch Back to the Master Branch**:
   - Switch back to the `main` (or `master`) branch:
     ```sh
     git checkout main
     ```

2. **Merge the New Branch**:
   - Merge the `feature/exercise-1` branch into the `main` branch:
     ```sh
     git merge feature/exercise-1
     ```

3. **Push the Changes to GitHub**:
   - Push the updated `main` branch to GitHub:
     ```sh
     git push origin main
     ```

### Step 7: Publish Your Project on GitHub

1. **Push Initial Commit to GitHub**:
   - Push the initial commit to GitHub (if not done already):
     ```sh
     git push -u origin main
     ```

### Step 8: Update Your Portfolio

1. **Add More Content**:
   - Add more sections to your `index.html` like "Skills" or "Contact".
   - Update the CSS to improve the styling.

2. **Commit and Push Changes**:
   - Whenever you make changes, remember to commit and push them to GitHub:
     ```sh
     git add .
     git commit -m "Describe your changes"
     git push
     ```

3. **Review Changes**:
   - Use GitHub to review the history of your changes and understand how version control helps in managing your project.
   - add me as your Reviewer and do not merge your PR, if I approved the PR I will let you know so that you can merge it automatically

**Bonus**:
- Experiment with advanced CSS features like flexbox, grid, or animations.
- explore more css styles to make your website beautiful
- Use Git branches to experiment with new features or designs before merging them into the main branch.
- Go to extensions, install the ff
   - Live Server by Ritwick Day (to test your HTML via server)
   - CSS Peek by Pranay Prakash (to allow you to check class strings as definitions from html)

By following these steps, you will gain hands-on experience with creating a simple website using HTML and CSS while learning to manage your project with Git.
