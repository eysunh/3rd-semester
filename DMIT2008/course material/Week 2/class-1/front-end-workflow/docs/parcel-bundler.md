# Parcel Bundler
Before you start there are a few things you need to do to get parcel setup and working with your project.

## Flight  Check
1. Initalize you project folder to use node modules.
```console
    npm init
```
1. If your just learning you can skip all the fields and just create the package.json file using the following command.
```console
    npm init -y
```
1. If the project folder contains a package.json file and no node_modules directory then install all the required modules listed in the package.json file by running.  
```console
    npm install
```
1. Install parcel as a dev dependancy
```console
   npm install -D parcel
```
1. Install a simple http server I will be using http-serve
```console
   npm install -D http-serve
```


### Dev Build
To run parcel in development issue the following command from the  VS Code terminal
```console
   npx parcel src/index.html
```
<br/>
You should se the dev server started on localhost on port 1234
 
```
 Server running at http://localhost:1234  
 ✨ Built in 552ms
```

### Parcel Bundle For Production
By default parcel will bundle your project and place it into the dist folder. This is the folder you would deploy. To run parcel for production run the following command from the VS Code terminal.

```console
   npx parcel src/index.html
```
<br/>

You should see output in the terminal similar to this:

```
✨ Built in 949ms

dist/index.html            365 B    300ms
dist/index.17429a75.css     78 B    612ms
dist/index.5c90d6bb.js     134 B    122ms
 ```