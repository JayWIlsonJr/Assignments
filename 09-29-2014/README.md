# 09/29/2014
Write a page with a list of items (books, bands, whatever) and a search box (`<input type="search">`). Using test driven development, write a Backbone View that filters the list as you type.

- Write tests first!
- If you haven't yet, read the [bower home page](http://bower.io).
- Install Backbone using bower and include it in your page, keeping in mind that the comments that are in the yeoman scaffold have special meaning.

**Pro Tip**: A good way of organizing your list would be to have a single View that is in control of the `<ul>`, and a View that represents each `<li>`. The `<ul>` could have a `render` function that renders the `<ul>` and a `renderChildren(items)` method that renders the `<li>`s for either the whole list or a filtered list. Or, you can just render the children in your "glue code" if that seems too complicated.

## Bonus
- Read https://gcanti.github.io/2014/09/25/six-reasons-to-define-constructors-with-only-one-argument.html
- [TDD, where did it all go wrong](http://vimeo.com/68375232)

## Power Level 9000
- Try and add animations so that the items don't just blink out of existence as they're being filtered. A good way of doing this is to add a function to the view that animates it then removes it from the DOM. Some things to look into:
    - $.on('transitionend')
    - Backbone.View#remove
- Use tiny pizza server to fetch the items using AJAX. Then add create, update, and delete functionality.
