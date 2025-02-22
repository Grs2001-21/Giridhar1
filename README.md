"# Giridhar1" 

## Running Tests Locally

# 1. How to Set Up and Run Tests Locally
Prerequisites
Install Python 
Create and activate a virtual environment
Setup Instructions

# Clone the repository
git clone https://github.com/Grs2001-21/Giridhar1.git
cd Giridhar1

# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows (Git Bash)
source venv/Scripts/activate

# Install dependencies
pip install -r requirements.txt

# Run tests
pytest --disable-warnings --cov=app tests/


# 2. How CI/CD Pipeline Works
GitHub Actions is used for Continuous Integration (CI)
Workflow file is located at .github/workflows/test.yml
The pipeline triggers on push and pull requests to the main branch
Pipeline Steps:
Checkout Code: Fetches the latest code from GitHub
Set Up Python Environment: Installs Python 3.10
Install Dependencies: Installs project dependencies from requirements.txt
Run Tests: Executes tests using pytest and generates a coverage report

Final Steps
After making these updates, commit and push your changes:

git add README.md
git commit -m "Updated README with test setup and CI/CD details"
git push origin main

#### **How CI/CD Pipeline Works**
```md
## CI/CD Pipeline with GitHub Actions

### **Pipeline Triggers**
- Runs automatically on **push** and **pull requests** to the `main` branch.

### **Pipeline Steps**
1. **Check Out Code**  
   - Clones the repository.
   
2. **Set Up Python Environment**  
   - Installs Python 3.10 and dependencies.

3. **Run Tests**  
   - Executes all tests using `pytest` with coverage.

4. **Deploy (If Implemented)**  
   - Future enhancement: Auto-deploy on passing tests.

