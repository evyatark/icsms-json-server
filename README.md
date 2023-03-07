# json-server

## for ICSMS project


## How to run
### localy
```
node server.js
```
or any of:
```
npm run watch
npm run dev
npm run start
```

The above runs a json-server in localhost in port 8000!

to run on port 3005, do:
```
PORT=3005 npm run start
```

The default port is hard-coded as 8000 `server.js`, but can be overridden with PORT=...


The json-server serves the data that is hard-coded in the file `db.json`. This data includes ICSMS "products", and "investigations".

The json-server also serves image files stored in `./public` sub-directory. These are images of the products. The file name of each image is the uuid of the product.

http://localhost:8000/4dab8aaa-ba6a-4674-a273-f493b43981c8.jpeg can be used to get the file 4dab8aaa-ba6a-4674-a273-f493b43981c8.jpeg from the public sub-dir.
http://localhost:8000/icsms retrieves the whole icsms collection, 
http://localhost:8000/icsms/2 retrieves a single row (with id 2)


### Vercel
according to https://javascript.plainenglish.io/how-to-set-up-deploy-fake-rest-api-server-using-json-server-24e26dc1d120


## TO DO
add a public deployment in Vercel so that this data can be used by the public deployed application.
