# Shopify JSON Store Lister

## Architecture:
* /config/__settings.html__ adding the fieldset/section to theme settings file
* /layout/__theme.liquid__ adding the module to the Shopify theme, _by including:_
  * /snippets/__retailers.liquid__ javascript file. _It decodes the..._
  * /assets/__retailers_data.json__ _outputs it as an object in the..._
  * /templates/__page.retailers.liquid__ 	 alternate Page template _containing_
  * `div#retailers_placeholder`

## Dependencies
* [Jquery 1.8 or higher](http://jquery.com/)
* [Isotope](http://isotope.metafizzy.co/)
* [jQuery Selectbox plugin](https://code.google.com/p/select-box/)


### JSON file setup

``` json
[
  {
    "Name": "Tricky3",
    "Address": "PO Box 12345",
    "Address 2": "",
    "City": "Santa Barbara",
    "Province/State": "CA",
    "Country": "USA",
    "Postal/Zip Code": "78910",
    "Phone": "123.456.7890",
    "Fax": "",
    "Email": "mangling@tricky3.co.uk",
    "Website": "http://tricky3.uk/"
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

* 1 Drop Down Style, driven by [jQuery Selectbox plugin](https://code.google.com/p/select-box/)
* 2 Links-based, with collapsible groups
* 3 Full-list, with horizontal or vertical layout

### Features
Responsive Layout with configurable Breakpoints & Columns :: Script calculates automatically the width for each column
Options for hiding Retailers Outside the US, Online and/or Special Retailers
Aggregate data for Retailers Outside the US as well as for Special Retailers
Script automatically orders and groups the data by name and country 

### As seen on:

* [Twigs & Honey](http://tricky3.co.uk/blogs/portfolio/6695894)

#### Thanks to:

* [Blu Kicks](http://tricky3.co.uk/blogs/portfolio/6195786)
* [Zara Terez](http://tricky3.co.uk/blogs/portfolio/16820564)
