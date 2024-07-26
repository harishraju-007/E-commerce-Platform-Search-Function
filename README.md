
# E-Commerce Platform Search Function

This project demonstrates the implementation of search functionality for an e-commerce platform using Java. It includes both linear and binary search algorithms, providing a comparative analysis of their time complexities and suitability for different datasets.

## Features

- **Product Class**: Represents a product with attributes such as `productId`, `productName`, and `category`.
- **Linear Search**: Implements a simple search algorithm that iterates through the array to find a product.
- **Binary Search**: Implements a more efficient search algorithm that works on a sorted array of products.

## Project Structure

- `Product`: A class representing a product with attributes `productId`, `productName`, and `category`.
- `LinearSearch`: A class containing the linear search algorithm.
- `BinarySearch`: A class containing the binary search algorithm.
- `ECommerceSearch`: The main class that sets up the products and performs searches using both algorithms.

## Asymptotic Notation

- **Big O Notation**: Describes the upper bound of the time complexity of an algorithm.
  - **Linear Search**: O(n)
  - **Binary Search**: O(log n)

## Time Complexity Analysis

- **Linear Search**:
  - **Best Case**: O(1) - when the product is the first element in the array.
  - **Average Case**: O(n/2) - when the product is somewhere in the middle.
  - **Worst Case**: O(n) - when the product is the last element or not present.
  
- **Binary Search**:
  - **Best Case**: O(1) - when the middle element is the product.
  - **Average Case**: O(log n) - when the product is somewhere in the middle of the search interval.
  - **Worst Case**: O(log n) - when the product is not present.

## Usage

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/ecommerce-search-function.git
    cd ecommerce-search-function
    ```

2. **Compile and Run**:
    ```bash
    javac ECommerceSearch.java
    java ECommerceSearch
    ```

## Example

The `ECommerceSearch` class sets up an array of products and performs searches using both linear and binary search algorithms:

```java
Product[] products = {
    new Product(1, "Laptop", "Electronics"),
    new Product(2, "Smartphone", "Electronics"),
    new Product(3, "Shirt", "Clothing"),
    new Product(4, "Shoes", "Footwear")
};

// Linear Search
Product foundProduct = LinearSearch.linearSearch(products, "Smartphone");
System.out.println("Linear Search Result: " + (foundProduct != null ? foundProduct : "Product not found"));

// Binary Search
foundProduct = BinarySearch.binarySearch(products, "Smartphone");
System.out.println("Binary Search Result: " + (foundProduct != null ? foundProduct : "Product not found"));
```

## Conclusion

This project provides a clear comparison between linear and binary search algorithms and their suitability for different use cases in an e-commerce platform. It helps in understanding how to optimize search functionality for fast performance.

---
