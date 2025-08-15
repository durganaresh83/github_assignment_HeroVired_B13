# Steps: Integrate Git LFS for Large Binary Files
# 1. Install Git LFS
  choco install git-lfs
  
# 2. Initialize Git LFS in Your Repository
  cd git_assignment_HeroVired
  git lfs install

# 3. Create and Checkout the lfs Branch
  git checkout -b lfs

# 4. Track Large File Extensions with Git LFS
  git lfs track "*.zip"
  This will create or update the .gitattributes file in the repo.

# 5. Add Your Large File (>200MB) to the Repository
  Copy or move a large file (e.g., large_sample_file.zip) into the repo directory.

# 6. Stage and Commit Changes
  Add both the large file and the .gitattributes file:
  git add .
  git commit -m "Add large file with Git LFS tracking"

# 7. Push the Branch and Large File to GitHub
  git push origin lfs

# 8. Clone the Repository on Another Machine
  On a different machine (make sure Git LFS is installed there too):
  git clone -b lfs https://github.com/<your_username>/git_assignment_HeroVired.git
  cd git_assignment_HeroVired

 # 9. Verify Downloaded File
   List files and check size:
   1s -lh
   The large file should be fully downloaded (check the file size matches the original size).




