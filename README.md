# ShoppingApp

An Android shopping app showcasing a list of products using a `RecyclerView`. Users can browse a collection of products and view detailed information by selecting any item.

---

## Features

- Displays a list of products with name, price, and basic details.
- Uses `RecyclerView` with a `LinearLayoutManager` for efficient scrolling.
- Clicking on a product opens a details screen with more information.
- Simple, clean architecture with Kotlin and Android Jetpack components.

---

## Project Structure

- **MainActivity.kt**: Main screen displaying the list of products.
- **Product.kt**: Data model representing a product.
- **MyAdapter.kt**: RecyclerView adapter to bind product data to list items.
- **DetailsActivity.kt**: Activity to show detailed product information.
- **activity_main.xml**: Layout file containing the `RecyclerView`.

---

## Code Overview

In `MainActivity`, an ArrayList of `Product` objects is created and displayed in a `RecyclerView`. When a user clicks on an item, the app opens `DetailsActivity`, passing the selected product's details via an `Intent`.

```kotlin
val products = ArrayList<Product>().apply {
    add(Product("Semi Conductor Diodes", 2000.0, "diodes", "1", "Manufactured in a small town in China", "Black"))
    add(Product("Transistors", 700.0, "transistors", "2", "Manufactured in a small town in China", "Black"))
    add(Product("Watches", 300.0, "watches", "3", "USA MADE", "Red"))
    add(Product("Monitors", 400.0, "monitors", "4", "Manufactured in USA", "Blue"))
}
