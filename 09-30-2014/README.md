# 09/30/2014

Write a simple todo app that uses Backbone Views and Models. An example (actually written in Backbone) can be found [here](http://todomvc.com/architecture-examples/backbone/). Don't worry about all the UI flourishes, you should just be able to add, delete, and complete todos. A todo should have properties that track its name and whether it is complete, and your views should respond to changes in those properties. It will probably be best to use separate views for the list and the items, but you can use one view if you'd like.

Though we didn't really cover them in class, using a Backbone Collection would probably make this assignment a lot easier, if you want to look up how to use them. Of note, a collection takes an array of models, and you can search the collection for a particular model using underscore functions. A collection triggers events that are helpful for re-rendering your views.

```js
// make an array of Backbone models
var models = [new Backbone.Model({name: "Jake"}), new Backbone.Model({name: "Finn"})];
// Pass those models into the Collection constructor
var collection = new Backbone.Collection(models);
// To remove a single model, find it first.
var jake = collection.findWhere({name: "Jake"});
// Call .remove with the model.
// This will trigger a `remove` event on the collection
collection.remove(jake);
// Call .add with a model
// This will trigger an `add` event on the collection
collection.add(jake);
```
