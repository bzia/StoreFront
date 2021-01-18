# StoreFront - An E-Commerce Platform

- Now Live @ https://storefrontwebapp.herokuapp.com/
- Inspiration: A MERN Stack Udemy Project Course

## Main View
![screenshot](https://github.com/bzia/StoreFront/blob/master/storefrontPic.png)
## Features
- Product pagination + reviews/ratings
- Checkout process involving a sequence of screens and the PayPal Payments API to may for created orders
- Designated admins can sign in and make product/user/order changes straight to the DB
  - This allows the store owner to mark orders as delivered and manage items inventory/stock aswell 
## Usage

### Env Variables

Create a .env file in then root and add the following

```
NODE_ENV = development
PORT = 5000
MONGO_URI = your mongodb uri
JWT_SECRET = 'abc123'
PAYPAL_CLIENT_ID = your paypal client id
```

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


### Seeding The Database

The following commands (defined in package.json "scripts") can be used to wipe the user and product data or overwirte it with sample data.

```
# Fill db with sample users and products
npm run data:import

# Destroy data completely
npm run data:destroy
```

```
Sample User Logins

admin@example.com (Admin)
123456

john@example.com (Customer)
123456

jane@example.com (Customer)
123456
```
