# Text

You can add as much custom text as you like to any content page

## Text attributes

You can use text attributes to display short snippets of text/numeric values on your content pages

### Text snippets

A text snippet would be something like the following subheader, "the best suites on the web":

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/text-snippet-example.png)

Start by creating a new text attribute:

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-text-snippet-1.png)

Go to the content type and fill the new text attribute with the details you would like:

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-text-snippet-2.png)

Use the following code to retrieve the snippet:

`<h3>{{ content_subheader }}</h3>`

### Text blocks

A text block could be anything from an Excerpt to a lengthy description on a product or category.

The text blocks section looks like this:

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/text-block-example.png)

When you add a new text block, it will appear as a new header at the top of the tinyMCE box:

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/text-block-example-2.png)

You can call text blocks with the following code:

`{{ content_text_primary }}`

If you wanted to call the example one instead, your liquid code would be:

`{{ content_text_example }}`
