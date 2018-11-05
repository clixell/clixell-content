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

## Adding a custom theme to your tinyMCE

To add your own custom colours and styles to your TinyMCE text editor, you will need to overwrite the default one by uploading your own into the themes folder of your project.

A typical styles config will look like the following:

```
{
  "Stylesheets": [
    "https://cdn.shopify.com/s/files/1/1301/3681/t/2/assets/base.css"
  ],
  "Fonts": [
    "To Do"
  ],
  "Styles": {
    "Headings": {
      "Heading 1": "h1",
      "Heading 2": "h2",
      "Heading 3": "h3",
      "Heading 4": "h4",
      "Heading 5": "h5",
      "Heading 6": "h6",
      "Paragraph": "p",
      "Lead Paragraph": "p.lead",
      "Blockquote": "blockquote"
    },
    "Colors": {
      "Primary": ".primary",
      "Orange": ".orange",
      "Purple": ".purple",
      "Green": ".green",
      "Blue": ".blue",
      "Red": ".red",
      "White": ".white",
      "Black": ".black"
    },
    "Presets": {
      "No presets": ".null",
      "NEW PRESET": ".nul"
    },
    "Buttons": {
      "Primary": ".btn.btn-primary",
      "White": ".btn.btn-white",
      "Xlight": ".btn.btn-xlight",
      "Light": ".btn.btn-light",
      "Secondary": ".btn.btn-secondary"
    },
    "Images": {
      "Float Left": ".float-left",
      "Float Right": ".float-right"
    },
    "BlockFrames": {
      "Example 1": ".cxl-block-frame-example-1",
      "Example 2": ".cxl-block-frame-example-2"
    },
    "SliderFrames": {
      "Middle Center": ".cxl-slider-middle-center",
      "Middle Left": ".cxl-slider-middle-left",
      "Top Left": ".cxl-slider-top-left",
      "Top Center": ".cxl-slider-top-center"
    }
  }
}
```

You should call it `cxl-styles-config.json` and replace the stylesheets link at the top with your own stylesheet.
