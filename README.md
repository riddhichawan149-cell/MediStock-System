MediStock-System

Pharmacy Inventory & Prescription Billing API

MediStock is a Pharmacy Inventory and Prescription Billing System developed using Node.js, Express.js, Sequelize ORM, and MySQL. It manages patients, medicine stock, prescriptions, billing, and inventory reports.

Features

Patient management

Medicine inventory management

Prescription creation and billing

Automatic stock deduction after successful billing

Medicine search and low-stock identification

Inventory and sales reports

Input validation and error handling

Database transactions for prescription billing

Technologies Used

Frontend: React.js

Backend: Node.js and Express.js

ORM: Sequelize

Database: MySQL

Language: JavaScript

Requirements

Node.js 18 or newer

MySQL 8 or compatible version

npm

Installation

Clone the repository:

git clone https://github.com/riddhichawan149-cell/MediStock-System.git
cd MediStock-System

Install dependencies:

npm install

Copy .env.example to .env and configure your database credentials.

Run the database migrations:

npm run db:migrate

To insert demo data, run:

npm run db:seed

Start the backend:

npm start

The default API address is http://localhost:3000, provided the application is configured to use that port. The GET /health endpoint can be used to check the API status.

API Endpoints

Method

Endpoint

Description

GET

/health

Check API status

GET

/api/patients

List patients

POST

/api/patients

Create a patient

GET

/api/medicines

List or search medicines

POST

/api/medicines

Add a medicine

GET

/api/prescriptions

List prescriptions

POST

/api/prescriptions

Create a prescription and bill

GET

/api/reports/inventory

View inventory and sales reports

Project Structure

src/ – Backend source code.

src/controllers/ – Request handling.

src/models/ – Database models.

src/routes/ – API routes.

src/migrations/ – Database migrations.

src/seeders/ – Demo data.

test/ – Automated tests.

package.json – Dependencies and scripts.

.env.example – Sample environment configuration.

Testing

Run the automated tests:

npm test

Security

Never upload your real .env file or database passwords to GitHub.

Use appropriate database permissions.

Avoid using demo data in production.

Future Improvements

Deploy the frontend and backend online.

Connect the frontend to the deployed API.

Add authentication and user roles.

Improve dashboard and reporting features.