![WhatsApp Image 2025-02-14 at 20 33 38_16a4ea10](https://github.com/user-attachments/assets/5e5ffb13-6776-4e9d-82a9-cf5a1ef16608)
![WhatsApp Image 2025-02-14 at 20 33 38_54d943c1](https://github.com/user-attachments/assets/5dc56d9c-a22f-4ee9-98c7-39b493d9ad6b)
![WhatsApp Image 2025-02-14 at 20 33 38_0953a89a](https://github.com/user-attachments/assets/44d8063f-0d2f-4301-859d-43861e0ac84f)
![WhatsApp Image 2025-02-14 at 20 34 10_0f93cda8](https://github.com/user-attachments/assets/75dfd69b-c3da-433d-86bd-8979be8aa27e)
![WhatsApp Image 2025-02-14 at 20 42 33_7a849d86](https://github.com/user-attachments/assets/44fe8040-7f46-4120-ad56-8edbe1f3b68f)

## Features

- Full featured shopping cart
- Product reviews and ratings
- Top products carousel
- Product pagination
- Product search feature
- User profile with orders
- Admin product management
- Admin user management
- Admin Order details page
- Mark orders as delivered option
- Checkout process (shipping, payment method, etc)
- PayPal / credit card integration
- Database seeder (products & users)

## Usage

- Create a MongoDB database and obtain your `MongoDB URI` - [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register)
- Create a PayPal account and obtain your `Client ID` - [PayPal Developer](https://developer.paypal.com/)

### Env Variables

Rename the `.env.example` file to `.env` and add the following

```
NODE_ENV = development
PORT = 5000
MONGO_URI = your mongodb uri
JWT_SECRET = 'abc123'
PAYPAL_CLIENT_ID = your paypal client id
PAGINATION_LIMIT = 8
```

Change the JWT_SECRET and PAGINATION_LIMIT to what you want

### Install Dependencies (frontend & backend)

```
npm install
cd frontend
npm install
```

### Run

```

# Run frontend (:3000) & backend (:5000)
npm run dev

# Run backend only
npm run server
```

## Build & Deploy

```
# Create frontend prod build
cd frontend
npm run build
```

### Seed Database

You can use the following commands to seed the database with some sample users and products as well as destroy all data

```
# Import data
npm run data:import

# Destroy data
npm run data:destroy
```

```
Sample User Logins

admin@email.com (Admin)
123456

john@email.com (Customer)
123456

jane@email.com (Customer)
123456
```

---
