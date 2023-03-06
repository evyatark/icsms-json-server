# json-server

## for ICSMS project


### How to run
```
node server.js
```
This runs a json-server in localhost in port 3004!

The port is defined hard-coded in `server.js`!

The json-server serves the data that is hard-coded in the file `db.json`. This data includes ICSMS "products", and "investigations".

The json-server also serves image files stored in `./public` sub-directory. These are images of the products. The file name of each image is the uuid of the product.

## TO DO
add a public deployment in Vercel so that this data can be used by the public deployed application.
