# Supply Chain Optimization & Inventory Analysis for Salamate Gostar Pharma

## Project Overview

This project aims to optimize the supply chain operations and inventory management for a large pharmaceutical distribution company, "Salamate Gostar Pharma." The company faces challenges such as high inventory holding costs, stockouts, expired goods, and inefficient delivery times. This data-driven initiative seeks to address these issues by leveraging advanced analytics and simulation.

## Current Phase: Comprehensive Synthetic Data Generation

In the current phase, we have developed a robust framework for generating a comprehensive and realistic synthetic dataset that mirrors the complexities of a real-world pharmaceutical supply chain. This dataset is crucial for subsequent analysis, modeling, and optimization efforts.

### Generated Data Schemas:

The following dataframes are generated, representing various aspects of the supply chain:

* **`products_df`**: Master data for all pharmaceutical products, including `product_id`, `product_name`, `product_category`, `unit_price`, `avg_shelf_life_days`, and `storage_conditions`.
* **`warehouses_df`**: Master data for the company's 10 distribution warehouses, including `warehouse_id`, `warehouse_name`, `warehouse_city`, `latitude`, `longitude`, and `capacity_units`.
* **`suppliers_df`**: Master data for product suppliers, including `supplier_id`, `supplier_name`, `supplier_location`, `avg_lead_time_days`, and `reliability_score`.
* **`customers_df`**: Master data for customer pharmacies, including `customer_id`, `customer_name`, and `customer_location`.
* **`purchase_orders_df`**: Transactional data for product purchases from suppliers, including `po_id`, `po_date`, `supplier_id`, `product_id`, `ordered_quantity`, `unit_cost`, `expected_delivery_date`, `actual_delivery_date`, and `delivery_status`.
* **`sales_df`**: Transactional data for product sales to customers, including `sales_id`, `sales_date`, `customer_id`, `warehouse_id`, `product_id`, `sold_quantity`, `sales_price`, and `delivery_time_hours`.
* **`returns_df`**: Data for returned products, including `return_id`, `sales_id`, `return_date`, `product_id`, `warehouse_id`, `returned_quantity`, and `return_reason`.
* **`inventory_df`**: Simulated inventory snapshots over time for each product, warehouse, and batch, including `snapshot_date`, `warehouse_id`, `product_id`, `batch_number`, `quantity_on_hand`, and `expiry_date`.
* **`waste_df`**: Records of wasted inventory (primarily due to expiry), including `waste_date`, `warehouse_id`, `product_id`, `batch_number`, `wasted_quantity`, and `reason`.
* **`stockout_df`**: Records of stockout events (when demand exceeds available inventory), including `stockout_date`, `warehouse_id`, `product_id`, and `stockout_quantity`.

## How to Run

This project is developed in a Google Colab environment.

1.  Open the `01_data_generation.ipynb` notebook (or copy the provided code into a new Colab notebook).
2.  Run all cells sequentially.
3.  Ensure the `Faker` library is installed by running `!pip install Faker` in the first cell.

The generated DataFrames will be saved as `.csv` and `.parquet` files in your Colab environment.

## Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Faker** (for synthetic data generation)
* **datetime**

## Next Steps

The next phases of this project will involve:

* **Exploratory Data Analysis (EDA):** Deep dive into the generated data to uncover patterns, trends, and identify bottlenecks and inefficiencies.
* **Feature Engineering:** Creating new, meaningful features from the raw data for advanced modeling.
* **Demand Forecasting:** Building predictive models to forecast future product demand.
* **Inventory Optimization:** Developing strategies and models to determine optimal inventory levels across warehouses.
* **Cost Analysis & Business Impact:** Quantifying the potential savings and operational improvements resulting from the optimizations.

## Contribution

Feel free to explore the code, suggest improvements, or contribute to the project.

## License

This project is licensed under the MIT License.
