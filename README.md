# Vendor Management System

This is a Vendor Management System built using Django and Django REST Framework. The system allows you to manage vendors, track purchase orders, and evaluate vendor performance metrics.

## Getting Started

To get started with the project, follow these instructions:

1. Clone the repository to your local machine:
      git clone https://github.com/prudhvikollanapK/Fatmug.git

2. Navigate to the project directory:
      cd fatmug

3. Install project dependencies using pip:
      pip install -r requirements.txt

4. Run migrations to create the database schema:
       python manage.py makemigrations
       python manage.py migrate

5. Start the development server:
       python manage.py runserver

6. Database administration(optional):
       python manage.py createsuperuser

7. Access the application in your web browser at http://localhost:8000.


## API Endpoints

The project provides the following API endpoints:

- Vendor APIs:
- `POST /api/vendors/`: Create a new vendor.
- `GET /api/vendors/`: List all vendors.
- `GET /api/vendors/{vendor_id}/`: Retrieve a specific vendor's details.
- `PUT /api/vendors/{vendor_id}/`: Update a vendor's details.
- `DELETE /api/vendors/{vendor_id}/`: Delete a vendor.

- Purchase Order APIs:
- `POST /api/purchase_orders/`: Create a purchase order.
- `GET /api/purchase_orders/`: List all purchase orders.
- `GET /api/purchase_orders/{po_id}/`: Retrieve details of a specific purchase order.
- `PUT /api/purchase_orders/{po_id}/`: Update a purchase order.
- `DELETE /api/purchase_orders/{po_id}/`: Delete a purchase order.

- Historical Performance Report APIs:
- `POST /api/historical_performance/`: Create a historical performance report.
- `GET /api/historical_performance/`: List all historical performance reports.
- `GET /api/historical_performance/{historical_performance_id}/`: Retrieve details of a specific historical performance report.
- `PUT /api/historical_performance/{historical_performance_id}/`: Update a historical performance report.
- `DELETE /api/historical_performance/{historical_performance_id}/`: Delete a historical performance report.

- Vendor Performance Evaluation:
- `GET /api/vendors/{vendor_id}/performance/`: Retrieve a vendor's performance metrics.

## Postman APIs

For easier interaction with the APIs, you can use the provided Postman collection. Import the collection into Postman to access the following APIs:

- Fatmug Vendor Management System APIs: [FATMUG.postman_collection.json]

## Contributing

Contributions to the project are welcome! If you'd like to contribute, please fork the repository, make your changes, and submit a pull request. Please ensure that your code follows PEP 8 style guidelines and includes appropriate tests.
