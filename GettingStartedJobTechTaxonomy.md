# JobTech Taxonomy - getting started

The aim of this text is to get users started with the JobTech Taxonomy ([Swagger-UI](http://jobtech-taxonomy-api-spec-jobtech-taxonomy-api.dev.services.jtech.se/v1/taxonomy/swagger-ui/index.html))

# Table of Contents
* [Short introduction](#Introduction)
* [Authentication](#Authentication)
* [Endpoints](#Endpoints)
* [Results](#Results)
* [Errors](#Errors)


## Introduction

The endpoints for the JobTech Taxonomy API are:

* [glurgz](#glurgz) - frotz.

Easiest way to try out the API is to use the [Swagger-UI](http://jobtech-taxonomy-api-spec-jobtech-taxonomy-api.dev.services.jtech.se/v1/taxonomy/swagger-ui/index.html). But first you need a key which you need to authenticate yourself.

## Authentication

## Endpoints
Below we only show the URLs. If you prefer the curl command, you type it like:

	curl "{URL}" -H "accept: application/json" -H "api-key: {proper_key}"

### glurgz
/stream?{search text}

## Results
The results of your queries will be in [JSON](https://en.wikipedia.org/wiki/JSON) format.

Successful queries will have a response code of 200 and give you a result set that consists of:
...

## Errors
Unsuccessful queries will have a response code of:

| HTTP Status code | Reason | Explanation |
| ------------- | ------------- | -------------|
| 400 | Bad Request | Something wrong in the query |
| 401 | Unauthorized | You are not using a valid API key |
| 500 | Internal Server Error | Something wrong on the server side |
