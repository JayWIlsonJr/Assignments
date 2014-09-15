# 09/15/14

You should create an application, from scratch, that uses ajax to store, retrieve, update, and delete data from the tiny server API.
- It should use yeoman and the tiy-webapp generator to get started.
- It should use SCSS
- It should use Underscore templates
- It should be able to create objects using POST
- It should be able to retrieve objects using GET
- It should be able to delete objects using DELETE
- It should be able to update objects using PUT

The tiny server is available at http://tiny-pizza-server.herokuapp.com/

## Example
Creating a blog using the API.

- GET /collections/blog returns all the blog articles. I should be able to see a list of all the blog articles, both title and body (like a blog).
- POST /collections/blog creates a blog article. I should have a form that allows me to create a blog with a title and a body. It should have a "Save" or "Create" button.
- PUT /collections/blog/:id updates the blog with that id. I should have a form that allows me to edit the blog's title and body. It should have a "Save" or "Update" button.
- DELETE /collections/blog/:id deletes a blog with that id. Each article in the list should have a delete button that deletes the article.

### Optional
- GET /collections/blog/:id fetches that blog article. I could have blog titles in a list that, when click, load only that article into the page.

# Hints
If you want to use a form for your objects, you might find the [`.serializeArray` method](http://api.jquery.com/serializearray/) helpful. You will need to modify it's result to make it useable by the API (there's an iteration function that is great at turning an array of things into a single thing).

## serializeArray results
```js
[
  {
    name: "title",
    value: "My Cool Title"
  },
  {
    name: "body",
    value: "Some cool blog content."
  }
]
```

## tiny server expects:
```js
{
  title: "My Cool Title",
  body: "Some cool blog content."
}
```
