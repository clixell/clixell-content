# Adding a custom theme to your tinyMCE

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

You should name the json file `cxl-styles-config.json` and replace the stylesheets url with your own stylesheet.
