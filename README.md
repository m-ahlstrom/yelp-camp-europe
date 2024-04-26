# Yelp Camp Europe

## THIS PROJECT IS STILL IN DEVELOPMENT

## THIS README IS A DRAFT

Yelp Camp Europe is a web application built with Node.js, Express.js and MongoDB. This project is currently in development. Everything is functional: the basics of the authentication system, campground creation, reviews. What it needs is a little polishing, adding extra features. And deploying to Vercel. It was previously deployed to Render.

The code in this project is based on the [The Web Developer Bootcamp](https://www.udemy.com/course/the-web-developer-bootcamp/) course by Colt Steele from Udemy.

## Features

- Authentication system: register, login, logout.
- Create, edit or remove your campgrounds. Review other's campgrounds, edit or remove your reviews.

## Features Yet To Be Implemented

- Authentication. Use a valid e-mail address or a Google-account.
- Cannot create a campground without an image. A campground cannot have more than 5 images.
- User roles: hosts can create campgrounds, guests can book and review them.
- You can see your campgrounds, reviews, previous or upcoming bookings, change your password and even delete your account anytime with all related information.
- Booking system. Hosts and guests also get e-mails about the bookings.
- Geo-restriction: all campgrounds are in Europe.
- Sort campgrounds by reviews, price or location. Find campgrounds on a cluster map.
- Implement Cloudflare Turnstile as a Google reCaptcha alternative.

## Technologies

- Node.js: an open-source and cross-platform JavaScript runtime environment.
- Express.js: fast, unopinionated, minimalist back-end framework for Node.js.
- MongoDB: general-purpose document-based NoSQL database.
- Mongoose: a MongoDB object modeling tool designed to work in an asynchronous environment.
- Cloudinary: used as cloud-based storage for images.
- Mapbox: Google Maps-alternative map-provider.
- Vercel: hosting provider.

## Run it locally

1. Install [MongoDB](https://www.mongodb.com/). <em>Give more precise instructions for getting the MONGO_URL.</em>
2. Create a [Cloudinary](https://cloudinary.com/) account to get an API key and secret code.
3. Create a [Mapbox](https://www.mapbox.com/) account to get an API key.

```sh
git clone https://github.com/m-ahlstrom/yelp-camp-europe.git
cd yelp-camp-europe
npm install
```

1. Create a .env file in the root of the project and add the following:

```md
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_KEY=
CLOUDINARY_SECRET=
MAPBOX_TOKEN=
MONGO_URL=
```

Run `node app.js` in the terminal within the project directory.

Then go to [localhost:8060](http://localhost:8060/).
