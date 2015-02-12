# Shopify JSON Store Lister

Architecture: 
    	settings.html				(config) adding the fieldset to the settings file
    	
    	theme.liquid				(layout) adding the module to the Shopify theme, by including
    	retailers.liquid           	(snippets) is a javascript file. It encodes the
    	retailers_data.json        	(assets) as a JavaScript Object Notation (JSON) and outputs it as an object in the 
    	retailers_placeholder      	(div id) that is placed directly into the Shopify Page.
    	page.retailers.liquid      	(template) is simply used as the identifier for the whole structure to get initiated 
