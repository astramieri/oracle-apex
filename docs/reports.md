# APEX Reports

A report in APEX is the formatted result of a SQL query.

Different types of reports:
- Interactive Report
- Interactive Grid
- Classic Report
- Faceted Search
- Cards
- Smart Filters

Different ways of creating reports:
- when you create a new application
- when you create a new page
- when you create a new region
	- dragging from Gallery
	- using Rendering Tree Context Menu
	- using Gallery Context Menu

## Interactive Report

Interactive reports generates all the HTML markup on the server as a part of the APEX page. The data returned from the SQL query is rendered along with all other markup that makes up the UI, the toolbar, the dialogs, and everything.

An Interactive Report include:
- Search Bar
- Action Menu
	- Columns
	- Filter
	- Data
		- Sort
		- Aggregate
		- Compute
		- Flashback
	- Format
		- Control Break
		- Highlight
		- Rows Per Page
	- Charts
	- Group By
	- Pivot
	- Report
		- Save Report
		- Reset
	- Download
	- Subscription
- Column Header Menu
- Edit Icons

## Interactive Grid

Interactive reports generates all the HTML markup on the server as a part of the APEX page. The data returned from the SQL query is rendered along with all other markup that makes up the UI, the toolbar, the dialogs, and everything. The client-side behaviors are implemented in a single monolithic JavaScript module. 

In contrast, interactive grid does all the HTML rendering on the client. The server provides the data in JSON format.

## Classic Report

End Users cannot customize classic reports.

## Faceted Search

End user can set filters using facets on the left or upper side of the screen. A facet shows possible values together with the occurrence count within the result set. When an end user uses a facet, the results, dependent facets, and occurrence counts refresh immediately.

## Cards

A card page features colorful blocks which resemble index cards laid out on a page. A cards report region decoratively supports customization of layout, and appearance, and the illusion of icons, batches, media, and actions.

## Smart Filters

A smart filter page features a single search field with filters at the top of the page and a report. Each filter is displayed as a suggestion chip with a single count how often the specific suggestion value occurs.
