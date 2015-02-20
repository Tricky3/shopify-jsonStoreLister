# Shopify JSON Store Lister

## Architecture: 
* /config/__settings.html__ adding the fieldset/section to theme settings file
* /layout/__theme.liquid__ adding the module to the Shopify theme, _by including:_
  * /snippets/__retailers.liquid__ javascript file. _It decodes the..._
  * /assets/__retailers_data.json__ _outputs it as an object in the..._
  * /templates/__page.retailers.liquid__ 	 alternate Page template _containing_
  * `div#retailers_placeholder`
