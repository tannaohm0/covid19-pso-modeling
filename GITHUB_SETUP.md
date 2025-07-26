# GitHub Upload Guide

## Step 1: Create a GitHub Account (if you don't have one)
1. Go to [github.com](https://github.com)
2. Click "Sign up" and create your account
3. Verify your email address

## Step 2: Create a New Repository
1. Click the "+" icon in the top right corner of GitHub
2. Select "New repository"
3. Fill in the repository details:
   - **Repository name**: `covid19-pso-modeling` (or any name you prefer)
   - **Description**: "COVID-19 modeling using Particle Swarm Optimization (PSO) algorithm"
   - **Visibility**: Choose Public (recommended for portfolio)
   - **Initialize with**: Don't check any boxes (we'll upload existing files)
4. Click "Create repository"

## Step 3: Upload Your Project Files
### Option A: Using GitHub Desktop (Recommended for beginners)
1. Download and install [GitHub Desktop](https://desktop.github.com/)
2. Sign in with your GitHub account
3. Click "Clone a repository from the Internet"
4. Select your newly created repository
5. Choose a local path on your computer
6. Copy all your project files to this folder:
   - `PSO_assignment.ipynb`
   - `README.md`
   - `requirements.txt`
   - `.gitignore`
   - `LICENSE`
7. In GitHub Desktop, you'll see all the files listed
8. Add a commit message like "Initial commit: COVID-19 PSO modeling project"
9. Click "Commit to main"
10. Click "Push origin" to upload to GitHub

### Option B: Using Command Line (For advanced users)
1. Open Command Prompt (Windows) or Terminal (Mac/Linux)
2. Navigate to your project folder:
   ```bash
   cd "C:\Users\Ohm Tanna\Desktop\PSO PROJECT"
   ```
3. Initialize git repository:
   ```bash
   git init
   ```
4. Add all files:
   ```bash
   git add .
   ```
5. Make initial commit:
   ```bash
   git commit -m "Initial commit: COVID-19 PSO modeling project"
   ```
6. Add remote repository (replace with your actual repository URL):
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/covid19-pso-modeling.git
   ```
7. Push to GitHub:
   ```bash
   git push -u origin main
   ```

## Step 4: Verify Your Upload
1. Go to your GitHub repository page
2. You should see all your files listed
3. Click on `PSO_assignment.ipynb` to view your notebook
4. The README.md should display nicely on the main page

## Step 5: Add Dataset Information
Since the COVID-19 dataset is large, you should:
1. Add a note in your README about where to get the dataset
2. Or upload a sample dataset if it's small enough
3. Consider using GitHub LFS for large files if needed

## Step 6: Make Your Repository Stand Out
1. Add topics/tags to your repository (click "Manage topics")
   - Suggested tags: `covid19`, `pso`, `epidemiology`, `machine-learning`, `python`, `jupyter`
2. Add a repository description
3. Consider adding screenshots of your visualizations to the README

## Troubleshooting
- If you get authentication errors, you may need to set up SSH keys or use a personal access token
- If files are too large, consider using Git LFS or excluding them from the repository
- Make sure your `.gitignore` file is working properly to exclude unnecessary files 