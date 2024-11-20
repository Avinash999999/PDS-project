# Navigate to your project folder or create one
mkdir my-project
cd my-project

# Initialize Git
git init

# Create a README.md file
echo "# My Project" > README.md

# Add project details to the README
echo "## Description" >> README.md
echo "This is my final project. It demonstrates XYZ functionality." >> README.md
echo "## How to Run" >> README.md
echo "1. Install dependencies\n2. Run the main script" >> README.md

# Add other files to your project
mkdir src
echo "print('Hello, World!')" > src/main.py

# Create a .gitignore file to exclude unnecessary files
echo "__pycache__/" > .gitignore
echo ".env" >> .gitignore

# Stage all files for the first commit
git add .

# Commit your changes
git commit -m "Initial commit: Add project files and README"

# Connect to a remote repository (replace with your repo URL)
git remote add origin https://github.com/your-username/your-repo-name.git

# Push your local repository to GitHub
git branch -M main
git push -u origin main

