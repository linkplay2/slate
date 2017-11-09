---
title: Linkplay Mobile SDK Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - java
  - objective_c

toc_footers:
  - <a href='mailto:info@linkplay.com'>Have Questions or Suggestions?</a>
  - <a href='http://linkplay.com/'>Become a Linkplay Developer</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to the Linkplay Mobile SDK documentation page! You can use our SDK to access various functionalities and interact with devices powered by the Linkplay A-series modules, which currenty supports wifi-setup and various content playback abilities.

We have language bindings in JAVA and Android and Objective C for iOS! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

This example API documentation page was created with [Linkplay](https://www.linkplay.com). Feel free to edit it and use it as a base for your own API's documentation.

# AVS Authentication

> To authorize, use this code:

```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> Make sure to replace `meowmeowmeow` with your AVS authentication key.

The Linkplay SDK enables you to login to your Amazon account in order to retrieve the AVS access token. You can register a new AVS dev account key at Amazon's[developer portal](https://developer.amazon.com/alexa).

Amazon Alexa expects for the API token to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>

# Playback Control

## Get All Songs in Queue
```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get Current Song
```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

## Delete a Song in Queue
```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "deleted" : ":("
}
```

This endpoint deletes a specific kitten.

### HTTP Request

`DELETE http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to delete

# Music Player Control

## Play
```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Pause
```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

## Skip/Next
```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "deleted" : ":("
}
```

This endpoint deletes a specific kitten.

### HTTP Request

`DELETE http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to delete

# Device Information

## Get Device Status
```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get Wifi Information
```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

## Change Device Settings
```java
while(all && i < val.length()){
    c = val.charAt(i);
    all = c == '0' || c == '1';
    i++;
}
return all;
```

```objective_c
#import <Foundation/Foundation.h>

NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
NSLog (@"Hello, World!");
[pool drain];
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "deleted" : ":("
}
```

This endpoint deletes a specific kitten.

### HTTP Request

`DELETE http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to delete
