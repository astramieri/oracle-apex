# Shared Components

Shared components are common elements that can be displayed or applied on any page within an application.

## Navigation and Search

Common navigation controls are:

- **Lists**   
	
	A list is a shared collection of links. Each list element has a display condition that enables you to control when it displays. 
	
	You add a list to a page by creating a region and specifying the region type as a list.

	Oracle APEX supports two types of lists: static lists and dynamic lists (based on SQL query or a PL/SQL function executed at runtime)

- **Navigation Menu**
	
	A navigation menu is a list of links that enable users to navigate the pages in an application. Navigation menus are supported only in applications using the **Universal Theme**.

	Navigation menus support the creation of hierarchical submenus.

- **Breadcrumbs**

	A breadcrumb is a hierarchical list of links that display using templates. You can display a breadcrumb as a list of links or as a breadcrumb bar.

- **Navigation Bar Lists**

	navigation bar entries offer users a simple navigation path for moving between pages and an application. A navigation bar entry can be an image, an image with text beneath it or simply text search configurations.

- **Search Configurations**

	Search configurations contain information about a searchable data source. They can be referenced from search regions to add declarative searches in your application. Searches can be based on local data source, REST-enabled SQL service, REST data source, or predefined Oracle Text or Oracle APEX list.

	There are three types of searches supported:
	- Standard
	- List 
	- Oracle Text 