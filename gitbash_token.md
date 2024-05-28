1. Generate a Personal Access Token (PAT) on GitHub:
   - Go to your GitHub account settings.
   - Navigate to Developer settings > Personal access tokens.
   - Click on "Generate new token."
   - Give your token a name, select the scopes (permissions) you need, and click "Generate token."
   - Copy the generated token (it will be displayed only once).

2. Configure Git Bash to use the Personal Access Token:
   - Open Git Bash on your computer.
   - Set your GitHub username and email if you haven't already:
     ```
     git config --global user.name "Your GitHub Username"
     git config --global user.email "your-email@example.com"
     ```
   - Set the token as your password for GitHub:
     ```
     git config --global credential.helper store
     ```
   - Store the token using Git Bash (replace `YOUR_TOKEN` with your actual token):
     ```
     git credential-store --file ~/.git-credentials store << EOF
     protocol=https
     host=github.com
     username=YOUR_GITHUB_USERNAME
     password=YOUR_TOKEN
     EOF
     ```

3. Verify the configuration:
   - Test the connection by cloning a repository from GitHub:
     ```
     git clone https://github.com/username/repository.git
     ```
   - Git Bash should use the Personal Access Token for authentication without prompting for a password.
