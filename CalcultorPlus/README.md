# Step-by-Step Instructions
  1. Create GitHub repository
  Log in to your GitHub account.
  Click Create repository.

# 2. Clone repository to local system
  git clone https://github.com/<your-username>/git_assignment_HeroVired.git
  cd git_assignment_HeroVired
  
# 3. Create dev branch
  git checkout -b dev
  
# 4. Add the initial code
  Create file calculator.py:
  touch calculator.py
  update the python code

# 5.Commit and push to dev
  git add calculator.py
  git commit -m "Initial calculator code without square root implementation"
  git push -u origin dev

# 6.Merge dev into main for Version 1
  git checkout main
  git merge dev
  git push origin main
