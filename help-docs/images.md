  # Images

  ## Adding images to a Content page

  You can add all kinds of images to your content type, from Thumbnails to Jumbotrons. Here are some examples with guides on
  how to implement them.

  ## Thumbnails

  ![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/thumbnail-example.png "Example of a thumbnail")

  ---

  To upload a custom thumbnail to a content type, first start by altering the config of your content page, adding a new single image type to the image section with the title "Thumbnail":

  ![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-thumbnail-1.jpg)

  ---

  Then you should go to the pages content and find the Thumbnail handle, and upload your desired image:

  ![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-thumbnail-2.jpg)

  ---

  Call the thumbnail with the following:

  `<img src={{ item_image_thumbnail }}></img>`

  Complete.</strong> Your thumbnail will now appear.

  ## Galleries

  To add a gallery to a content type, first start by altering the config of your content page, adding a new multi image type to the image section with the title "Gallery":

  ![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-gallery-1.jpg)

  ---

  Find the gallery header in the content type and select as many images as you like:

  ![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-gallery-2.jpg)

  ---

  Print the gallery with the following:

  ```
  {% assign images = content_image_gallery | split: "<cxl>" %}
	{% assign images_alt = content_image_gallery_alt | split: "<cxl>" %}
	{% assign images_width = content_image_gallery_width | split: "<cxl>" %}
	{% assign images_height = content_image_gallery_height | split: "<cxl>" %}

	<div class='row'>
		{% for image in images %}
			<div class='col-sm-2 mb-4'>
				<a href="{{ image }}" target="_blank">
					<img src="{{ image }}?crop=240x160" alt="{{ images_alt[forloop.index0] }}" title="{{ images_alt[forloop.index0] }}" class="img-fluid" />
				</a>
				<code>size: {{ images_width[forloop.index0] }}x{{ images_height[forloop.index0] }}</code>
			</div>
		{% endfor %}
	</div>
  ```

  Complete. Your gallery will now appear.

  ## Jumbotron

  ![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/jumbotron-example.png)

  ---

  To upload a jumbotron to a content type, first start by altering the config of your content page, adding a new single image type to the image section with the title "Jumbotron":

  ![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-jumbotron-1.jpg)

  ---

  Upload your jumbotron image:

  ![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-jumbotron-2.jpg)

  ---

  Call the jumbotron with the following code:

  `<img src='{{ content_image_jumbotron }}?crop=1920x300' class="img-fluid" />`

  Or

  `<img src='{{ content_image_jumbotron }}?fit=1920x300' class="img-fluid" />`

  ## Image GET variables

  You may have noticed the variable "crop" in the image src. There are two options you can pass in when pulling out an image, "crop" and "fit".

  ### Crop

  Crop will crop the image to fit the size specified.

  ### Fit

  Fit will force the image to fit the box specified.
