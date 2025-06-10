# cloudkitchen

# Cloud Kitchen Platform

A comprehensive cloud kitchen management platform with multi-tenant support, real-time order tracking, and integration with major food delivery aggregators.

## Features

- Multi-tenant Account Management
  - Admin Dashboard
  - Kitchen Operator Interface
  - Vendor/Supplier Portal
  - Customer Portal

- Authentication & Security
  - Two-Factor Authentication
  - Role-based Access Control
  - Session Management

- Core Functionality
  - Kitchen Management
  - Menu Management
  - Inventory Tracking
  - Order Processing
  - Dispatch Management
  - Real-time Updates

- Payment Integration
  - Stripe
  - PayPal

- Aggregator Integration
  - Talabat UAE
  - Zomato
  - Noon
  - Deliveroo

## Tech Stack

### Backend
- Django 5.0
- Django REST Framework
- Channels (WebSocket)
- Celery (Task Queue)
- PostgreSQL
- Redis

### Frontend
- React (Admin Dashboard)
- React Native (Mobile App)
- Flutter (Mobile App)

## Setup Instructions

1. Clone the repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

5. Run migrations:
   ```bash
   python manage.py migrate
   ```

6. Create superuser:
   ```bash
   python manage.py createsuperuser
   ```

7. Run the development server:
   ```bash
   python manage.py runserver
   ```

## Project Structure

```
cloudkitchen/
├── backend/                 # Django backend
│   ├── accounts/           # User management
│   ├── kitchen/            # Kitchen operations
│   ├── orders/             # Order management
│   ├── inventory/          # Inventory tracking
│   ├── payments/           # Payment processing
│   └── aggregators/        # Delivery platform integrations
├── frontend/               # React admin dashboard
├── mobile/                 # React Native & Flutter apps
└── docs/                   # Documentation
```

## API Documentation

API documentation is available at `/api/docs/` when running the development server.

## Contributing

Please read CONTRIBUTING.md for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the LICENSE file for details. 
