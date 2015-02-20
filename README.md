# Shopify JSON Store Lister

## Architecture: 
* settings.html (config) adding the fieldset to the settings file
* theme.liquid (layout) adding the module to the Shopify theme, by including
  * __retailers.liquid__ 	      (snippets) is a javascript file. It encodes the
  * __retailers_data.json__   	(assets) as a JavaScript Object Notation (JSON) and outputs it as an object in the 
  * __retailers_placeholder__ 	(div id) that is placed directly into the Shopify Page.
  * __page.retailers.liquid__ 	(template) is simply used as the identifier for the whole structure to get initiated 