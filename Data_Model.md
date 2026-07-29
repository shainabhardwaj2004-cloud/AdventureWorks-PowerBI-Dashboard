# Data Model

## Model Design

This project follows a Star Schema data model, which improves report performance and simplifies DAX calculations.

---

## Fact Tables

### Sales Data
Contains transactional sales information including revenue, orders, customers, products, and territories.

### Returns Data
Stores product return information for return rate analysis.

---

## Dimension Tables

- Calendar Lookup
- Customer Lookup
- Product Lookup
- Territory Lookup
- Product Categories
- Product Subcategories

---

## Relationships

The Sales Data table is connected to all lookup tables through one-to-many relationships.

The Returns Data table is linked with Product Lookup for return analysis.

The Calendar Lookup table enables time intelligence calculations such as Previous Month, YTD, and Rolling Period analysis.

---

## Benefits of the Model

- Faster report performance
- Reduced data redundancy
- Improved scalability
- Simplified DAX calculations
- Efficient filtering across visuals
- Better business analysis through organized relationships

---

## Modeling Techniques Used

- Star Schema
- One-to-Many Relationships
- Lookup Tables
- Fact Tables
- Calendar Table
- Dedicated Measure Table