# Quote Request Web Application

A Laravel-based quote request and management system. Specially designed for requesting quotes for the purchase and installation of windows, doors, and their accessories. The system automatically generates the quote and sends it as a PDF to the applicant's email address.

## Features

- Quote request form: Option to specify windows, doors, and their parameters and accessories by room.
- Automatic quote generation.
- Sending the quote as a PDF via email.
- Admin panel to manage incoming requests.
- Updating database prices from an Excel spreadsheet.

## Installation

### 1. Clone the Repository

First, clone the project to your local machine:

```bash
git clone https://github.com/palomaweb/WinDoorCalc.git
```

### 2. Install Composer

The project requires Composer for dependency management. If it is not installed, use the following command to install it:

```bash
composer install
```

### 3. Set Up Environment File

Create the .env file using the following command:

```bash
cp .env.example .env
```

Then, generate the application key:

```bash
php artisan key:generate
```

### 4. Set Up Database

Configure the database connection in the .env file according to your database settings.

### 5. Run Migrations

Run the migrations to create the database structure:

```bash
php artisan migrate
```

### 6. Start the Development Server

Start the built-in development server:

```bash
php artisan serve
```

The server will be available by default at http://localhost:8000.

## Usage

1. Visit the homepage of the web application.
2. Fill in the quote request form with information about windows, doors, and other products.
3. Click the "Request Quote" button.
4. The system will automatically generate the quote and send it as a PDF to the provided email address.

## Testing

The project includes test scripts, which can be run using the following command:

```bash
php artisan test
```

This will run the tests and check if the system works correctly.

## License

This project is intended solely for viewing and demonstration purposes. 
You may not modify, distribute, or use this project for commercial purposes.