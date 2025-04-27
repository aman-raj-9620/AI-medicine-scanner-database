# AI-medicine-scanner-database

CREATE DATABASE pharmacy_db;
USE pharmacy_db;

CREATE TABLE products (
    product_id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    category VARCHAR(50),
    price DECIMAL(10,2),
    quantity INT,
    stock INT,
    description TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP

INSERT INTO products (name, category, price, quantity, stock, description)
VALUES (
    'Paracetamol 500mg Tablet',
    'Pain Relief',
    1.50,
    100,
    200,
    'Used to treat mild to moderate pain and fever.'
);
select* from products;
