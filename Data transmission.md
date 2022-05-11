---
aliases: 
tags: digital
---
# Data transmission
## Network layer

Data stream can be unicast, multicast or broadcast

- Unicast: 1-1 device to device connection
- Multicase: Data exchange with numerous but specific clients
- Broadcast: Data exchange to any number of clients

## Application layer

Also known as session layer

Transmission can be synchronous or asynchronous

- Synchronous: sender and receiver take turns sending and acknowledging data
- Asynchronous: no acknowledgement of data

Data can be transmitted in many formats, 2 most common are XML and JSON

## Rest (representational state transfer)
**Re**presentational **S**tate **T**ransfer (REST) is a client-side architecture for using internet resources at a specific URI.

Generally uses JSON or XML, but can sometimes use CSV or other formats.

Uses some HTML syntax for ease of use

## JSON (javascript object notation)

JSON is a syntax for storing and exchanging data.

Is stored in plain text files

JSON is language independent, even though it uses JS syntax. JSON can be read by any programming language.

### Sending data with JSON

Data stored in a JS object can easily be converted to JSON and sent to a server. Likewise, data received in JSON format can be converted to a JS object.

#### Example send code

```javascript
var myObj = {name: "Jason", age: 31, city: "New York"};
var myJSON = JSON.stringify(myObj);
window.location = "demo_JSON.php?x=" + myJSON;
```

### JSON syntax

JSON syntax is derived from JS object notation syntax:

- Data is in key-value pairs: `"name":"John"`
- Pairs are separated by commas
- Curly braces hold objects
- Square brackets hold arrays

A property of an object can be accessed using dot notation:

```javascript
person.name; // returns "Jason"
```

#### Data types

JSON has the following data types:

- String
	- Must be written in double quotes
	- `{ "name":"Jason" }`
- Number
	- Can be integer or floating point
	- Written without double quotes
- Array
- Boolean
- JSON object
- Null

## XML (extensible markup language)

XML is a markup language much like HTML. It was designed to store and transport data and be self-descriptive.

XML DOES NOTHING!

XML is just information wrapped in tags. Software is needed to interpret these tags.

### Example XML

```xml
<note>  
    <to>Tove</to>  
    <from>Jani</from>  
    <heading>Reminder</heading>  
    <body>Don't forget me this weekend!</body>  
</note>
```

#### Differences between XML and HTML

HTML was designed to carry data with a focus on how it looks.

XML was designed to carry data with a focus on what the data is.

XML does not have any predefined tags like HTML does.

### XML Syntax

XML documents for a tree structure where each element is a child of the one above it (other than the root element) and can have children one level below it. Use indenting to indicate these.

A **prolog** defines the XML version and the character encoding:

```xml
<?xml version="1.0" encoding="UTF-8"?> 
```

UTF-8 is the default encoding for XML documents.

The next line is the **root element** of the document:

```xml
<bookstore>
```

The root element is mandatory and unique to the document.kkkkkk

The next line starts a `<book>` element:

```xml
<bookstore>
	<book category="cooking">
```

The `<book>` elements have four child elements:
```xml
<bookstore>
	<book category="cooking">
		<title lang="en">Everyday Italian</title>  
		<author>Giada De Laurentiis</author>  
		<year>2005</year>  
		<price>30.00</price>
```

The next line ends the `<book>` element:
```xml
</book>
```

All elements must have a closing tag (`</tag>`)

XML tags are case sensitive. The tag `<Letter>` is different to the tag `<letter>`.

