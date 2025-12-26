Solution: Git and GitHub Challenge (Week 4)
👤 Participant Information
Name: [Your Name]

Batch: DevOps Batch 9

GitHub Profile: [Link to your profile]

🛠 Task 1: Fork and Clone
Action: Forked the repository from LondheShubham153/90DaysOfDevOps.

Command used:

Bash

git clone https://github.com/[Your-Username]/90DaysOfDevOps.git
cd 2025/git/01_Git_and_Github_Basics
📂 Task 2: Local Repository Setup
Created directory week-4-challenge.

Initialized Git and created info.txt.

Commands used:

Bash

mkdir week-4-challenge && cd week-4-challenge
git init
echo "Hello, I am [Your Name], a DevOps enthusiast!" > info.txt
git add info.txt
git commit -m "Initial commit: Add info.txt with introductory content"

🔑 Task 3 & 4: Authentication and History
Remote Configuration: Added origin with Personal Access Token (PAT).

Log Verification: Viewed history to confirm the commit.

Commands used:

Bash

git remote add origin https://[USERNAME]:[PAT]@github.com/[USERNAME]/90DaysOfDevOps.git
git push -u origin main
git log --oneline
Commit Hash: [Paste your commit hash here]

🌿 Task 5: Branching and Feature Updates
Created a feature branch.

Modified the file and pushed.

Commands used:

Bash

git checkout -b feature-update
# (Edited info.txt)
git add info.txt
git commit -m "Feature update: Enhance info.txt with additional details"
git push origin feature-update


🧠 Why Branching Strategies Matter
In collaborative development, branching strategies are essential because:

Isolation: They keep experimental or "in-progress" code away from the stable main branch.

Parallelism: Multiple developers can work on different features (Feature A, Feature B) at the same time without overwriting each other's work.

Code Quality: Pull Requests allow for code reviews on a specific branch before the code is merged into production.

Conflict Management: It reduces the risk of merge conflicts by organizing changes into logical chunks.

🚀 Bonus: SSH Authentication
Action: Generated SSH keys and updated the remote URL.

Commands used:

Bash

ssh-keygen -t ed25519 -C "your_email@example.com"
git remote set-url origin git@github.com:[Your-Username]/90DaysOfDevOps.git
git push origin feature-update