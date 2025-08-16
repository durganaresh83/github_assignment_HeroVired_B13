# Geometry Calculator with Git Stash Workflow

# 1. Clone the GitHub Repository

# 2. Create the New Branch geometry-calculator
  git checkout -b geometry-calculator

# 3. Update the python code

# 4. Create a branch for Circle Area feature
  git checkout -b feature/circle-area

# 5. Implement the Circle Area feature
  Edit the geometry_calculator.py and complete the circle area part.

# 6. Stash incomplete Circle Area changes
  If the implementation is not yet completed, stash the changes without committing
  git stash

# Feature 2: Rectangle Area

# 1. Create a branch for the Rectangle Area feature
  git checkout -b feature/rectangle-area geometry-calculator

# 2. Implement the Rectangle Area feature
Edit geometry_calculator.py and complete the rectangle part:
if __name__ == "__main__":
    calculator = GeometryCalculator()
    length = 10
    width = 6
    print(f"The area of the rectangle with length {length} and width {width} = {calculator.calculate_rectangle_area(length, width)}")

# 3. Stash incomplete Rectangle Area changes
  git stash save "WIP: Rectangle area feature"

# Returning to Circle Area to Complete Work
# 1. Switch back to Circle Area branch
  git checkout feature/circle-area

# 2. Retrieve Circle Area stashed changes
  git stash apply

# 3. Complete the Circle Area implementation
  Commit and Push Circle Area

# Returning to Rectangle Area to Complete Work

# 1. Switch back to Rectangle Area branch
  git checkout feature/rectangle-area

# 2. Retrieve Rectangle Area stashed changes
  git stash apply

# 3. Complete the Rectangle Area implementation
  Commit and Push Rectangle Area

# Creating Pull Requests

# Go to GitHub repository
In the repository, you’ll see a message offering to create a pull request for feature/circle-area.

Click Compare & Pull Request.

Select base branch: dev and compare branch: feature/circle-area.

Add a title like: "Feature: Circle Area", description, and submit.

Repeat the same for:

feature/rectangle-area branch → Pull request into dev.

# Review & Merge
  Ask a teammate to review the PRs.

# Merge into dev
After approval → Click Merge pull request → Confirm.






