# Report on MLOps Deployment from PROD to DEV

# Objective:
The goal of this exercise was to simulate the deployment process from a development environment (DEV) to a production environment (PRD). One participant acted as the developer, responsible for pushing code, while the other played the role of the gatekeeper, ensuring the code worked correctly.

⸻

# Steps Followed:
	1.	Forming Pairs:
We split into pairs as instructed, and one of us assumed the role of the developer while the other took on the gatekeeper role.


	2.	Developer Role:
The developer followed these steps:
	•	Created a new project or used an existing one.
	•	Copied the code to a folder (which would be initialized as a git repository).
	•	Set up a virtual environment (venv) and installed necessary packages.
	•	Created a requirements.txt file to list all dependencies.
	•	Initialized a Git repository using git init.
	•	Added files to the repository (excluding the venv folder).
	•	Committed changes with the message “Initial commit”.
	•	Pushed the project to a remote git repository (e.g., GitHub or GitLab).
	•	Created a pull request (PR) to submit the changes.


	3.	Gatekeeper Role:
The gatekeeper reviewed the pull request and:
	•	Ensured the code was correct and met the requirements.
	•	Merged the pull request if everything looked good.
	•	Pulled the latest changes using git pull origin main.
	•	Set up a new virtual environment and installed the required dependencies using pip install -r requirements.txt.
	•	Ran the project to ensure it functioned correctly.


	4.	Swap Roles:
After completing the process once, we swapped roles and repeated the steps so that both of us gained experience as both the developer and the gatekeeper.

⸻

# Challenges Encountered:
	•	Git Push Issues:
While pushing the project to the remote repository, I faced issues with git push not working smoothly at first. This was mainly due to misconfiguration of the remote origin or authentication issues. The problem was resolved after verifying the remote URL and using the correct git push command.


	•	Python Version Conflict:
The project requirements specified using Python 3.11.11, but I initially had Python 3.12 installed, and later tried to install 3.11.11 on macOS. However, due to configuration issues and version management limitations, I was only able to successfully use Python 3.11.9 with pyenv. Despite this version being slightly earlier than required, it worked without causing compatibility issues in the project.

⸻

# Conclusion:

The exercise provided valuable hands-on experience simulating a real-world deployment flow using Git, virtual environments, and dependency management. It also highlighted the importance of version control and environment consistency, especially when working in teams. Communication between the developer and the gatekeeper was essential for resolving issues and ensuring a smooth deployment process.