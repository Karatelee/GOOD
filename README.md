CREATE TABLE Categories (
    CategoryID INT PRIMARY KEY AUTOINCREMENT,
    CategoryName TEXT
);

CREATE TABLE Products (
    product_id INT PRIMARY KEY AUTOINCREMENT,
    productName TEXT,
    price INT,
    categoryID INT REFERENCES Categories(id) IN DELETE SET NULL
);

CREATE TABLE Orders (
    OrderID INT PRIMARY KEY,
    OrderDate REAL,
    CustomerName TEXT
);
# GOOD
