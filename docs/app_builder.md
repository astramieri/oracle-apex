# APP Builder

## APEX Application

It is an HTML interface that exists on top of database objects such as tables or procedures.

It is a collection of pages linked together using navigation menus, tabs, buttons, or hypertext links.

## Application Page

A page is the basic building block of an application.

Every application consists of one or more pages.

To view a rendered version of your application, you submit it to the APEX Engine. The APEX engine dinamically renders and processes pages based on data stored in database tables.

Each page:
- can have buttons and fields (called items) that are grouped together into containers called **regions**;
- can include application logic (or processes);
- can branch to another page using conditional navigation.

You can view and edit a page in **Page Designer**, a fully featured integrated development environment.

## How the APEX Engine renders and processes pages

When you run an APEX application, the APEX engine relies on two processes:

1. **Show Page** is a page rendering process that assemble all the page attributes (including regions, items and buttons) into a viewable HTML page;
2. **Accept Page** performs forms page processing, including computations, validations, processes and branching.

You can use conditions in a application to control how pages and page components display and when processes, computations, and validations execute.

## Application UI

**Universal Theme** is a user interface for Oracle APEX. 

Universal Theme Advantages:

- Responsive Design
- Versatile User Interface
- Easy Customization

## Session State Management

Session state enables developers to store and retireve values for a user as the user navigates between different application pages.

APEX transparently maintains session state and provides developers with the ability to get and set session state values from any page in the application.

A **session ID** is a unique number assigned a specific user for the duration of that user's visit (session). The most visible location of the session ID is in the URL for a page request.

A session is a logical construct that establishes persistence (or stateful behavior) across page views. APEX sessions are logically and physically disting from Oracle Database sessions used to service page requests.

## URL Syntax

APEX applications support two types of URL syntax:
- (new) **friendly URL** Syntax (starting with APEX release 20.1)
- (old) **f?p** Syntax

Friendly URL Syntax creates a URL structure that identifies the address of Oracle APEX, the application, the page and uses standard web parameter syntax.

Structure:

	https://hostname:port/ords/r/path_prefix/app_alias/page_alias?parameters

Example:

	https://example.com:8080/ords/r/mycompany/hr-app/update-employees?session=13766599855150
