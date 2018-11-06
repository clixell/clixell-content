# Downloads

You can add downloads to your pages for the customer to download. You may want to use this feature to create a sizing guide, for example.

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/downloads-example.jpg)

## How to add Downloads

Go to your config and check "show downloads" in the options

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-downloads-1.jpg)

**Make sure you click save in the top right after making this change**

Go back to your content type and the new downloads section will now show

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-downloads-2.jpg)

Click "add new". Enter a title and upload your file. Ensure that "Status" is set to "Published"

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-downloads-3.png)

Click save.

In your template, you can call your new download(s) with:

```  
{% assign downloads = content_downloads | split: "<cxl>" %}
{% for download in downloads %}
<br/>{{ download }}
{% endfor %}
```

This code will be the same whether you have one download or multiple. We added another sizing guide for the US, here is what our
customer will now see:

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-downloads-5.png)
