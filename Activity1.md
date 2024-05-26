# Collaboration Activity Guide

## Step 1: Identify a Small Group
1. **Form a Group:**
   - Find 3-4 people to collaborate with for this exercise.
   - Ensure everyone has a GitHub account.

## Step 2: Create a Repository
1. **One Person Creates a Repository:**
   - One member from each group should log in to their GitHub account.
   - Click on the "+" icon in the top-right corner and select "New repository."
   - Fill in the repository details:
     - **Repository name:** Choose a meaningful name.
     - **Description:** Optionally, add a brief description.
     - **Public or Private:** Choose the visibility. For collaboration purposes, public is often easier.
     - **Initialize with a README:** Check this box if you want to add a README file.
   - Click "Create repository."

2. **Give Access to Group Members:**
   - Navigate to the repository's main page.
   - Click on the "Settings" tab.
   - In the left sidebar, click "Manage access."
   - Click on the "Invite a collaborator" button.
   - Enter the GitHub usernames of your group members and send the invitations.

## Step 3: Collaborators Accept the Invitation
1. **Accept the Invite:**
   - Each invited member will receive a notification on GitHub.
   - Click on the notification or go to the repository page and accept the invitation.

## Step 4: Clone the Repository
1. **Clone the Repository:**
   - Open a terminal or Git Bash on your local computer.
   - Navigate to the directory where you want to clone the repository.
   - Use the `git clone` command followed by the repository URL. You can find the URL on the repository page (click the green "Code" button to see it).
     ```sh
     git clone https://github.com/username/repository-name.git
     ```
   - Replace `https://github.com/username/repository-name.git` with the actual URL of your repository.

2. **Verify the Cloning:**
   - After the cloning process is complete, navigate into the repository directory:
     ```sh
     cd repository-name
     ```
   - List the files to ensure that the repository has been cloned successfully:
     ```sh
     ls
     ```

## Example Commands
Here’s an example of what the commands might look like:
```sh
# Cloning the repository
git clone https://github.com/johndoe/collab-project.git

# Navigating into the cloned repository
cd collab-project

# Listing the files to verify
ls
