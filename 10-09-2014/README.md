# 10/09/2014

The assignment is to make a [Slack](http://slack.com) clone called Crack.

- Use the firebase url https://crack.firebaseio.com/rooms/
- At minimum, have chats go to the 'general' room (`/rooms/general`)
- By default, emberfire uses the model name for the url, but you can change it using 'pathForType'. See [docs](https://github.com/firebase/emberfire).
- I should have to log in so that my chat messages have my username on them

## Optional
- Use the localStorage adapter to store the logged in user in localStorage.
- Create multiple rooms. Hint: To list the rooms, you can use the following code:
```js
    var ref = new Firebase("https://crack.firebaseio.com/rooms/");
    ref.once('value', function(data){
      data.forEach(function(room){
        console.log(room.name());
      });
    });
```
- Use the gravatar API to add avatar images.
- Use [marked](https://github.com/chjj/marked) to allow Markdown formatting in messages.
- Create an image tag if the message is a gif.
