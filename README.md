## Project Overview
Project Name: Midterm SYSARCH32
This is a midterm project that implements a CRUD-based MVC application using Laravel. It includes two main modules: colleges and departments, both performing basic CRUD operations.

## Steps to Clone and Run the Application
1. Clone the Repository
git clone https://github.com/biskiu/midterm_sysarch.git

2. Navigate to Project Directory
cd midterm_sysarch

3. Install Dependencies
composer install

4. Set Up Environment
- Copy the .env.example file:
cp .env.example .env
- Generate the application key:
php artisan key:generate

5. Configure Database
Update the .env file with your database credentials:
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=collegedb
DB_USERNAME=root
DB_PASSWORD=

Run database migrations:
php artisan migrate

6. Run the Application
php artisan serve
Visit http://127.0.0.1:8000 to access the application.

## Git Workflow Explanation
1. Cloning the Repository
git clone https://github.com/biskiu/midterm_sysarch.git

2. Creating a New Branch
Always create a new branch for feature development or bug fixes:
git checkout -b feature/branch-name

3. Making Changes and Committing
- Stage changes:
git add .
- Commit changes:
git commit -m "feat: add authentication"

4. Pushing Changes to GitHub
Push your branch to the repository:
git push origin feature/branch-name

5. Creating a Pull Request (PR)
- Go to your GitHub repository.
- Click Compare & Pull Request.
- Add a description and submit the pull request for review.

6. Code Review and Merging
- The project maintainer will review the PR.
- Once approved, the PR is merged into the main branch.
- After merging, delete the branch:
git branch -d feature/branch-name

## Best Practices
- Use descriptive branch names: feature/login, bugfix/typo-fix
- Write clear commit messages: feat: add login functionality
- Regularly pull updates:
    git pull origin main
