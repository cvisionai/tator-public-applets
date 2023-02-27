# Taxonomy Helper Applet

This applet uses the WoRMs rest API to allow a user to populate Localization attributes by selecting an item from a taxonomic tree.

## Project Notes

This applet are built for projects using the following setup:

Media attribute:
* Organism Name

Localization attributes:
* Scientific Name
* Rank
* Kingdom
* Family
* Class
* Phylum
* Order
* Genus
* Species
* Habitat

## Sidear applet
This is meant to work in the sidebar of the annotation view. Follow registration step below.

### To register this applet
Use the project settings page, or python tools to upload this file to a project as an applet. The required category is: "annotator-tools"

See docs for more info:
https://www.tator.io/docs/developer-guide/dashboards/create-annotator-menu-applets#registering-applets

### UX Notes
To use this applet you must first select an existing localization and then click the "book" icon in the annotator tools along the left side icon sidebar.

Note: When the icon appears during initialization, then it is ready to hear a localization selection. If for some reason the applet is initialized after you select you need to click off and reselect to populate the panel.

### Using the applet
It shows a taxonomic tree and default will populate the search based on the Media's "Organism Name" attribute. The selected item(s) populates the "Data preview" tab. The "Data preview" tab shows the populated attribute panel and shows the option to "Apply" the data. The the localization will be saved with the data going to the corresponding attributes by the same name (see above). When the post is successful you will see a message and an event sent to the annotation page will refresh the attribute panel to reflect the new data.




