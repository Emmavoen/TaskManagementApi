# TaskManagementApi
A task management application built using node.js
# Setup Instructions for TaskManagementAPI
## Prerequisites
Node.js (v14 or higher)
PostgreSQL
Git

## Steps
1. Clone the repository:
git clone <repository-url>
cd <File_directory >
2. Install dependencies:
npm install
3. Set up environment variables:
Create a .env file in the root directory and add the following variables:
PORT=5000
DOMAIN_NAME=localhost
DB_NAME= TaskManagementApi
DB_PASSWORD= YOUR_PASSWORD
DB_USER= YOUR_DB_USER
DB_HOST=localhost
4. Configure the database:
Make sure PostgreSQL is running and create a database named TaskManagementApi.
5. Run database migrations:
npm run migrate
6. Start the server:
npm run dev
7. The server should now be running on http://localhost:5000.
## API Endpoints
Create Task: POST /tasks
Get Tasks: GET /tasks
Update Task: PUT /tasks/:title
Delete Task: DELETE /tasks/:title
## Additional Scripts
Undo last migration:
npm run down
## Notes
Ensure that the PostgreSQL credentials in the .env file match your local setup.
You can modify the database configuration in config.js.
