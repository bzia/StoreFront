# StoreFront - An E-Commerce Platform

- Now Live @ https://storefrontwebapp.herokuapp.com/
- Inspiration: A MERN Stack Udemy Project Course

## Main View
![screenshot](https://github.com/bzia/StoreFront/blob/master/storefrontPic.png)
## Features

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

## Build & Deploy

```
# Create frontend prod build
cd frontend
npm run build
```

There is a Heroku postbuild script, so if you push to Heroku, no need to build manually for deployment to Heroku

### Seed Database

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
