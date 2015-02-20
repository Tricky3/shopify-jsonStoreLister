# Shopify JSON Store Lister

## Architecture: 
* settings.html (config) adding the fieldset to the settings file
* theme.liquid (layout) adding the module to the Shopify theme, by including
  * /snippets/__retailers.liquid__ javascript file. _It decodes the..._
  * /assets/__retailers_data.json__ _outputs it as an object in the..._
  * /templates/__page.retailers.liquid__ 	 alternate Page template _containing_
  * `div#retailers_placeholder`
