# Todo API

A [Web API](https://en.wikipedia.org/wiki/Web_API) with [ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/introduction-to-aspnet-core).

## How to use

```sh
# Clone the repo
git clone https://github.com/daltonbr/TodoApi.git

# Run the project locally
$ dotnet run

# Consume the API with Postman or a Browser (check Overview bellow)
https://localhost:5001/api/TodoItems

```

## Objectives

* Create a basic web API project.
* Add a model class and a database context.
* Scaffold a controller with CRUD methods.
* Configure routing, URL paths, and return values.
* Call the web API with Postman.
* At the end, having a web API that can manage "to-do" items stored in a database.  (DB _in memory_ for this example)

## Overview

This tutorial creates the following API:

API | Description | Request body | Response body
---|---|---|---
GET    | `/api/TodoItems`      | Get all to-do items     | None       | Array of to-do items
GET    | `/api/TodoItems/{id}` | Get an item by ID       | None       | To-do item
POST   | `/api/TodoItems`      | Add a new item          | To-do item | To-do item
PUT    | `/api/TodoItems/{id}` | Update an existing item | To-do item | None
DELETE | `/api/TodoItems/{id}` | Delete an item          | None       | None 

## The Architecture

![Architecture](./Documentation/Architecture.png)

## Credit and tools

* [.NET Core 3.1 SDK or later](https://dotnet.microsoft.com/download/dotnet-core/3.1)
* Based on this [Microsoft tutorial](https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-web-api).
