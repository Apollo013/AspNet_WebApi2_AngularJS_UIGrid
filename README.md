# AspNet_WebApi2_AngularJS_UIGrid

---
### Description

Another small app containing an AngularJS web client that accesses resources through a Web Api 2 service. 
This app demonstrates a host of features listed below. Hosted on Azure.

The primary goal of this is to show you how to implement the AngularJS UI-Grid plugin, and demonstrate how to page, sort and filter data on the server, rather that requesting all data from the server and allowing UI-Grids internal implementation to do these for us. A form is provided for creating & updating (validation included), and the ability to remove a record is also available. (Although not on the live site)

This app also demonstrates other features including DI, security, logging & design patterns.

Before you start, you will need to specify a database connection in your Web.config file.

---

Developed using Visual Studio 2015 Community

---

####Frameworks / Plugins / Languages

| No.        | Description  |
| -----------|-------------|
| 1 | ASP.NET Web Api 2 |
| 2 | OWIN |
| 3 | Entity Framework 6.1.0 |
| 4 | Ninject |
| 5 | Dynamic Linq |
| 6 | AngularJS, ngRoute, ngAnimate - 1.4.9 |
| 7 | AngularJS Toaster |
| 8 | AngularJS Loading Bar |
| 9 | AngularJS UI-Grid |
| 10 | Hoe HTML Template |
| 11 | CSS Bootstrap V4 alpha |
| 12 | jQuery |
| 13 | C# |
| 14 | Linq |
| 15 | Code First - Fluent Api |
| 16 | HTML |
| 17 | Microsoft.ApplicationInsights |
| 18 | Log4Net |
| 19 | JUnit |

---

####Server-Side Features

| Description |
|-------------|
| Extension Methods |
| Forcing Https Requests |
| IQueryable(T) extension method that uses Dynamic Linq for Dynamic sorting of queries |
| IQueryable(T) extension method that uses Dynamic Linq for Dynamic filtering of queries |
| Paging with Linq |
| OWIN setup & configuration |
| Attribute Routing |
| Repository, Unit of Work & Model Factory Patterns. |
| Dependancy Injection |
| Configuring domain entity tables using 'EntityTypeConfiguration' with ef migrations. |
| Creating custom 'IHttpActionResult' responses |
| Unit Testing with JUnit |
| Generic Repository |
| Exception Handling |
| Use of Reflection to check property names passed to controllers via url |
| Logging using Microsoft.ApplicationInsights.Log4NetAppender |
| Recursion |
| CORS Enabled to accept only a single client from making requests, plus specifying which verbs to accept |
| Authorize attribute used to authorize access to specific endpoints |
| CRUD functionality & Data validation |

---

####AngularJS Features

| Description  |
|-------------|
| AngularJS $Http Interceptor for configuring Requests & response errors |
| Making Restful calls in AngularJS using $http.post, put, get, delete |
| Solving the Angularjs 404 routing error using the web.Config file (see admin client) |
| External Pagination with UI-Grid |
| External Sorting with UI-Grid |
| External Filtering with UI-Grid |
| Displaying non-blocking notifications using Toastr |
| Displaying loading bar during http requests |
| Form validation using AngularJS |
| Routing using ngRoute |

---

####Structure

| No.        | Project Name        | Project Type  | Description  |
| -----------| ---------------- |-------------| -------------|
|1 | AdminClient     | Empty Web Project | Web User Interface |
|2| BusinessServices      |  Class Library      | Business logic layer that communicates between the web api and repositories |
|3| DataAccessLayer | Class Library      | Responisible for communicating with the database |
|4| DataService | Web Api 2 | Our web api data service |
|5| Models.DomainEntities | Class Library | Models used for constructing our database tables |
|6| Models.ViewModels | Class Library | View models used for sending information to the client |
|7| Repositories | Class Library | Repository layer |
|8| UnitTests | Unit Test | Testing |

---

####Resources
| Title | Author | Publisher |
|-------|--------|-----------|
|[UI-Grid-Info](http://ui-grid.info/docs/#/tutorial)| | UI Grid |
|[System.Linq.Dynamic](https://dynamiclinq.codeplex.com/)| | CodePlex |
|[Dynamic LINQ](http://weblogs.asp.net/scottgu/dynamic-linq-part-1-using-the-linq-dynamic-query-library)| Scott Guthrie | ScottGu's Blog |



