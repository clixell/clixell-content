# Calling data through ajax

You can bring any data stored in your clixell app in to your shopify store using ajax. This method means that you don't have to
call our app directly and can instead offer a service that looks like it is being created by your store.

## How to call data through ajax

An example of an ajax request would be something like the following:

`$("[cxl-content-testimonials]").load("/apps/cxl-content/testimonials/tag/Show+On+Homepage?view=homepage&items=1&random=true");`

This would be placed in the javascript and would load anything with a tag of "show on homepage" from the testimonials on the home page.

## The GET Variables

### view
This will declare the type of view to use

### items
Declares how my items to get from the specified content (testimonials in the example above)

### random
Declares whether to select a random item on each page load. If set to true, in the example above we would see a different testimonial
every time we loaded the home page (providing theres more than one testimonial to choose from).
