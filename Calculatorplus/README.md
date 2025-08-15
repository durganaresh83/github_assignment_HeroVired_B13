# Step-by-Step Instructions
# Clone repository to local system
  git clone https://github.com/<your-username>/git_assignment_HeroVired.git
  cd github_assignment_HeroVired_B13

#  Create dev branch
  git checkout -b dev

# Add the initial code
  Create file calculator.py
  update the python code

# Commit and push to dev

# Merge dev into main for Version 1
  Create Release v1 on GitHub:
  Go to repository → Releases → Draft a new release.
  Tag: v1.0
  Title: Version 1
  Description: Initial version without square root.
  Click Publish release.

# Create a branch for the new feature
   git checkout -b feature/sqrt
   Update the changes in the code
   
# Create Pull Request (feature/sqrt → main)
  Go to GitHub repo.
  Click Compare & pull request.
  Base: main, Compare: feature/sqrt.
  Add description → Create pull request.

# Request code review
`In the PR page, click Reviewers → add your classmate.

# Merge feature/sqrt into dev
  Once PR approved:
  git checkout dev
  git merge feature/sqrt
  git push
  
# Test in dev
  python calculator.py
  
# Merge into main and create Version 2
  git checkout main
  git merge dev
  git push
  
# Create Release v2 on GitHub:
  Tag: v2.0
  Title: Version 2
  Description: Added square root + fixed divide bug.
  Publish the release.
