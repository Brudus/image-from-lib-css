# ImageFromLibCss

This project uses a local library (image-with-lib-css) via verdaccio and tries to load a CSS file with an image included via `content: url()`.

## Setup

1. Publish the library locally and then install it from there in this project. (`npm install` won't work right now as the library is not available).
1. Run this project via `ng serve`. 

## What did work

For me it worked to copy over the files from the library to the assets folder of the application and using a CSS class that includes the image from the assets. In the library, I then only used `content: ('/arrow-down.svg');`