# Recommendation Cards

## Description

This can be used to quickly craft a set of recommendation cards.

## Screenshots
![](../images/pe-recommendation-cards-1.png)

## Additional Information/Notes

Uses ServiceNow® [Service Catalog](https://docs.servicenow.com/bundle/istanbul-it-service-management/page/product/service-catalog-management/concept/c_ServiceCatalogManagement.html)

---

## Installation

Download and install update set **[pe-recommendation-cards.u-update-set.xml](https://github.com/platform-experience/serviceportal-widget-library/blob/master/pe-recommendation-cards/pe-recommendation-cards.u-update-set.xml)** <br/><br/>
After installation, the widget can be accessed via the `Service Portal > Widgets` section for use and customization.<br/>
* SN Product Documentation - ['Load a customization from a single XML file'](https://docs.servicenow.com/bundle/istanbul-application-development/page/build/system-update-sets/task/t_LoadCustomizationsFromAnXMLFile.html)

---

## Configuration

Widget Option Schema parameters:

**"Title"** Widget Title. `Default: Recommended for You`<br/>
**"Category"** This is for defining a category `Default: PE My Devices`<br/>
**"Fields"** This is for defining the field items to display for the catalog item, using a comma separated list. For example: sc_cat_item.icon, sc_cat_item.name, etc. `Default: sc_cat_item.name, sc_cat_item.icon, sc_cat_item.short_description`<br/>
**"Items"** This is for defining the catalog items for display. If the "Show All Catalog Items" option is set to true, it will override this option. `Default: GL Reporting, empasiegel1, Office 2016`<br/>
**"Highlight"** This is for highlighting items, which adds a background color to the item or items using a comma separated list. For example: Office 2016, GL Reporting, etc. `Default: Office 2016`<br/>
**"Show Title"** This option will show the title if checked (true); if unchecked (false), will hide the title. `Default: true`<br/>
**"Show All Catalog Items"** This option will return all catalog items for a category, if checked (true). If unchecked (false), will only return the defined option Items. `Default: false`<br/>

---

## Platform Dependencies

### SN System Tables
* sc_cat_item
* sc_cat_item_category
* sc_category

---

## Sample Data and Data Structures

> See 'Configuration' above

---

## API Dependencies

<i>Dependencies are included and configured as part of the provided Update Set.</i>
> None

---

## CSS/SASS Variables

_CSS/SASS variables are given default values that can be overridden with theming or portal-level CSS._
> None