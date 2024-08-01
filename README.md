- 👋 Hi, I’m @mihirsavla
Here's a basic `README.md` file template for your project. You can customize it further based on your project's specific details and requirements.

```markdown
# Invoice Generator

## Overview

The Invoice Generator is a web application for creating and managing invoices. It allows users to select products, apply discounts, and generate PDF invoices. The application uses Node.js with Express for the backend and Puppeteer for PDF generation. The frontend is built using HTML, CSS, and JavaScript.

## Features

- Select product categories and products.
- Input product details including MRP, discount, and quantity.
- Add products to the invoice and view a summary.
- Remove products from the invoice.
- Download the invoice as a PDF.

## Technologies Used

- **Backend**: Node.js, Express
- **Frontend**: HTML, CSS, JavaScript
- **Database**: MySQL
- **PDF Generation**: Puppeteer
- **Version Control**: Git

## Installation

### Prerequisites

- Node.js (>= 14.0.0)
- MySQL (>= 8.0)

### Clone the Repository

```bash
git clone https://github.com/username/repository.git
cd repository
```

### Install Dependencies

```bash
npm install
```

### Set Up the Database

1. Create a MySQL database named `invoiceDB`.
2. Use the following SQL script to create the necessary table:

    ```sql
    CREATE TABLE products (
        id INT AUTO_INCREMENT PRIMARY KEY,
        name VARCHAR(255) NOT NULL,
        mrp DECIMAL(10, 2) NOT NULL,
        discount DECIMAL(5, 2) NOT NULL,
        quantity INT NOT NULL,
        discounted_price DECIMAL(10, 2) NOT NULL,
        total_price DECIMAL(10, 2) NOT NULL,
        unique_id VARCHAR(36) NOT NULL
    );
    ```

### Configure Environment Variables

Create a `.env` file in the root directory and add your MySQL credentials:

```env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_DATABASE=invoiceDB
```

### Start the Application

```bash
npm start
```

Visit `http://localhost:3000` in your browser to use the application.

## Deployment

### GitHub Repository

The source code for this project is hosted on GitHub. You can view or contribute to the project at:

[GitHub Repository](https://github.com/username/repository)

### Deployment on Vercel

1. Log in to [Vercel](https://vercel.com) and create a new project.
2. Connect your GitHub repository to Vercel.
3. Vercel will automatically detect that your project is a Node.js app and deploy it.

## Usage

1. **Select a Category**: Choose a product category from the dropdown.
2. **Select a Product**: Choose a product from the category.
3. **Enter Details**: Input MRP, discount, and quantity.
4. **Add Product**: Click the "Add Product" button to add the product to the invoice.
5. **View Summary**: View the list of added products and the total amount.
6. **Download PDF**: Click the "Download PDF" button to download the invoice as a PDF.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or issues, please contact [your-email@example.com](mailto:your-email@example.com).
```

### Notes:

- **Replace placeholders** like `username/repository` with your actual GitHub username and repository name.
- **Update environment variables** and other configuration details as needed based on your project's setup.
- **Include any additional sections** such as a detailed setup guide or FAQ if necessary.

Feel free to modify this template to better fit your project's needs.
