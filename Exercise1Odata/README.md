# Northwind OData API Query Examples

This exercise examples of how to interact with the Northwind OData API to retrieve data using various queries.

## Overview

The **Northwind OData API** is a demo service that provides access to a sample database containing data about products, customers, orders, and employees. Using OData, you can query this data with advanced filtering, sorting, and expansion features.

## Base URL

The base URL for the Northwind OData service is:

https://services.odata.org/northwind/northwind.svc

## Exercise Queries
<ul>
    <li>Get all orders with the client's details</li>
    <li>Get all employees who report to manager n° 2</li>
    <li>Get all products that are in stock</li>
    <li>Get only the names and code of product of the items that are not in stock</li>
    <li>Get only the top 5 most expensive products</li>
    <li>Find the orders that were shipped to Germany</li>
    <li>Get only the name and price of products which correspond to the "Beverage" category</li>
</ul>

## How to test

<div style="margin-left: 30px">

Use your favourite endpoint tester: Postman, ThunderClient, etc and paste the base URL.

Use the different extensions to query the appropiate collection and use query parameters to apply filtering, sorting or others to your preference.


</div>

## Parameters used


<ul>
  <li><b>$filter:</b> To filter the results by a criterion.</li>
  <li><b>$select:</b> To only select the properties of the base response that you would need to use.</li>
  <li><b>$top:</b> To limit the response to only the first 5 results.</li>
  <li><b>$orderby:</b> To sort the response by a criterion. At the moment the response returns a string therefore it is not working correctly. In a real world environment the selected criterion would need to be parsed to a number.</li>
  <li><b>$expand:</b> To add to the base result, the related entities from another collection that match the base response. In this example we get the Orders that correspond to a Client's ID as a Client may have multiple Orders.</li>
  <li><b>$format:</b> To format the response. This is optional. Should you want to keep the base format in XML, remove the parameter at the end of the query.</li>
</ul>




## Additional information

For more parameters please refer to the ODATA documentation here


<a href="https://www.odata.org/documentation/" target="_blank">Odata Documentation</a>

