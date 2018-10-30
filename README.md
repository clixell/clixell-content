# clixell-content

Clixell Content is a shopify app that does foo bar moo..

# Getting Started

1. Download the default liquid files from this repository
2. Open the app in admin and click "config"

The Name should be set to the name of the content type you are creating, eg. "Featured Products"

The Handle is what will be used to grab the content type in the browser and will create a link between the app and the liquid files.

4. Scroll down to the Text Editor box and type "Hello, world"

5. Once you have given your content type a handle, you should replicate and rename the downloaded liquid files to mirror this, replacing the "default" in the name with your handle. So, if your handle is "featured", the file name for the listing page would be:

cxl-content-default-listing.liquid --> cxl-content-featured-listing.liquid

Do the same for the other three templates, then upload these to the snippets directory of your project.

Go to: 
https://mystore.myshopify.com/apps/cxl-content/featured

You will be met by a blank page with "Hello, World." on it. You have now configured your listing page.
