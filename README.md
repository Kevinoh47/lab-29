![CF](http://i.imgur.com/7v5ASc8.png) LAB
=================================================

## Lab 29 Component Composition

### Author: Kevin O'Halloran

### Links and Resources
* [repo](https://github.com/Kevinoh47/lab-29)
* [Lab 29 Exercise 1 sandbox](https://codesandbox.io/s/nrzkowqv20)
* [Lab 29 Exercise 2 sandbox](https://codesandbox.io/s/549mpxo2mx)

### Modules Assignment 1
Assignment 1 focusses on composing an application with functional components in various ways.

#### `list.js`
##### Exported Values and Methods
The /src/components/lists.js file exports a functional component that returns a ul element thant renders props.children, should any exist in a child component that it may wrap.

#### `stuff.js`
##### Exported Values and Methods
The /src/components/stuff.js is a functional component that renders a ul element with a collection of li elements extracted from an object variable via Object.keys({}).map. 

It also imports the Things component and renders it.

This functional component exports itself.

#### `things.js`
##### Exported Values and Methods
The /src/components/things.js file builds the Things functional component and exports it. This component contains an object which it iterates over and returns as a list.

#### `index.js`
##### Exported Values and Methods
The /src/index.js file creates the App class and renders it. It is also the entry point into the application, defining the root element and rendering App under the root element.

The App class composes the application. It holds a list of songs in state, iteratests over it, and renders the resulting list as children of an imported List component. It also imports and renders a Stuff element.

It also contains a few opening Span tags. I confess I did not understand the instructions of what i was supposed to do with these spans.


### Modules Assignment 2
Assigment 2 focusses on converting functional components to class-based components.

#### `list.js`
##### Exported Values and Methods
The /src/components/lists.js file exports a functional component that returns a ul element thant renders props.children, should any exist in a child component that it may wrap.

#### `playlist.js`
##### Exported Values and Methods
The /src/components/playlst.js file creates a class-based component that creates a state object of songs by various artists. It has a render() method which iterates over the state object to create a list of artists and songs, then renders them as children of a List component. 

#### `stuff.js`
##### Exported Values and Methods
The /src/components/stuff.js converts the original functional component to a class-based component that renders a ul element with a collection of li elements extracted from an object variable via Object.keys({}).map. 

It also imports the Things component and renders it.

This class component exports itself.

#### `things.js`
##### Exported Values and Methods
The /src/components/things.js file converts the original Things functional component to a class component and exports it. This component contains an object which it iterates over and returns as a list.

#### `index.js`
##### Exported Values and Methods
The /src/index.js file creates the App class and renders it. It is also the entry point into the application, defining the root element and rendering App under the root element.

The App class composes the application. This version is cleaner that the previous version, merely composing the application based on imported components.

It also contains a few opening Span tags. I confess I did not understand the instructions of what i was supposed to do with these spans.


#### Running the app

* Endpoint: `https://codesandbox.io/s/nrzkowqv20`
  * Assignment 1 uses more functional components.
* Endpoint: `https://codesandbox.io/s/549mpxo2mx`
  * Assignment 2 uses more class-based components. App just composes the application from other components.


#### UML
Link to an image of the UML for your application and response to events
