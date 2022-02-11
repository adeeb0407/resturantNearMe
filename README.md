# resturantNearMe

## This is a NodeJS Application where as in you will find resturants Near you as far as you mention it.

### Setup

1)Have a `.env` file created and do as Follows in the file

DB_URL = {database URL} (name the collection `resturants`)
PORT  = {which ever port you wish for the app to run in}

2)Database JSON data will be avaliable in the `databseJSON.txt` file nad you will have to use Robo.3t to or any framework to insert them into your collection

3) `db.getCollection('restaurants').createIndex({ location: "2dsphere" })` run this command in your NOSQL Framework to get the sphere topology 

5) now just rtpe `npm start` in terminal and your good to GOO!!!

### Bonus Info

4) Take this data as Body

`{
    "latitude": 18.645368,
    "longitude" : 74.058112,
    "raduis" : 500
}`

and run it on postman with a post request add the url http://localhost:{your Port mentioned in .env file}/nearme

