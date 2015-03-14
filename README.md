# Shopify JSON Store Lister

## Architecture:
* /config/__settings.html__ adding the fieldset/section to theme settings file
* /layout/__theme.liquid__ adding the module to the Shopify theme, _by including:_
  * /snippets/__retailers.liquid__ javascript file. _It decodes the..._
  * /assets/__retailers_data.json__ _outputs it as an object in the..._
  * /templates/__page.retailers.liquid__ 	 alternate Page template _containing_
  * `div#retailers_placeholder`

### JSON file setup

``` json
[
  {
    "Name": "Tricky3",
    "Address": "PO Box 12345",
    "Address 2": "",
    "City": "Santa Barbara",
    "Province\/State": "CA",
    "Country": "USA",
    "Postal\/Zip Code": "78910",
    "Phone": "123.456.7890",
    "Fax": "",
    "Email": "mangling@tricky3.co.uk",
    "Website": "http:\/\/tricky3.com\/"
  },
  {
    // etc.
  }
]
```
__notes__
* trailing slashes should be escaped
* designate `"Country": "ONLINE"` for online-only retailers
* designate `"Province\/State": 'SPECIAL'` for special retailers

### View Options

* 1
* 2
* 3

### As seen on:

* [Twigs & Honey](http://tricky3.co.uk/blogs/portfolio/6695894)

#### Thanks to:

* [Blu Kicks](http://tricky3.co.uk/blogs/portfolio/6195786)
* [Zara Terez](http://tricky3.co.uk/blogs/portfolio/16820564)
