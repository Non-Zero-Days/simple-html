## Simple HTML

### Prerequisites:
Today's prerequisites will include notepad and an internet browser such as chrome or edge.

### Loose Agenda:
Create a simple website layout with HTML
Apply styling to our website via CSS
Apply bootstrap CSS styling to our website

### Step by Step
Create a directory to store this exercise in

Open Notepad and enter the following code
```
<!DOCTYPE html>
<html>
  <body>
    <div>
      <input type="text"/>
      <input type="submit"/>
    </div>
  </body>
</html>
```

Save the file to your selected directory as simple.html

Add a class to the submit control
```
<!DOCTYPE html>
<html>
  <body>
    <div>
      <input type="text"/>
      <input type="submit" class="primary"/>
    </div>
  </body>
</html>
```

Add a blue background style to the submit control
```
<!DOCTYPE html>
<html>
  <body>
    <div>
      <input type="text"/>
      <input type="submit" class="primary" style="background: blue"/>
    </div>
  </body>
</html>
```

Save and view the output by double clicking the simple.html file (this should open the file in a browser)

Adjust the background style to powderblue
```
<!DOCTYPE html>
<html>
  <body>
    <div>
      <input type="text"/>
      <input type="submit" class="primary" style="background: powderblue"/>
    </div>
  </body>
</html>
```

Extract the style to a style node within the html file then save and open the file in your browser to see the result
```
<!DOCTYPE html>
<html>
  <style>
    .primary {
      background: powderblue
    }
  </style>
  <body>
    <div>
      <input type="text"/>
      <input type="submit" class="primary"/>
    </div>
  </body>
</html>
```

Extract the style to it's own file and save it as simple.css
```
.primary {
  background: powderblue
}
```

Link the simple.css file in your simple.html code then view the result in your browser
```
<!DOCTYPE html>
<html>
  <link rel="stylesheet" href="simple.css"/>
  <body>
    <div>
      <input type="text"/>
      <input type="submit" class="primary"/>
    </div>
  </body>
</html>
```

Retrieve the latest CSS link from [Bootstrap](https://getbootstrap.com/docs/4.5/getting-started/introduction/) and use it to replace our link
```
<!DOCTYPE html>
<html>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/css/bootstrap.min.css" integrity="sha384-TX8t27EcRE3e/ihU7zmQxVncDAy5uIKz4rEkgIXeMed4M0jlfIDPvg6uqKI2xXr2" crossorigin="anonymous">
  <body>
    <div>
      <input type="text"/>
      <input type="submit" class="primary"/>
    </div>
  </body>
</html>
```

Change the class of our submit control to "btn btn-primary" and view the results in the browser
```
<!DOCTYPE html>
<html>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/css/bootstrap.min.css" integrity="sha384-TX8t27EcRE3e/ihU7zmQxVncDAy5uIKz4rEkgIXeMed4M0jlfIDPvg6uqKI2xXr2" crossorigin="anonymous">
  <body>
    <div>
      <input type="text"/>
      <input type="submit" class="btn btn-primary"/>
    </div>
  </body>
</html>
```

Congratulations on a non-zero day!


### Resources
- [Bootstrap - Getting Started](https://getbootstrap.com/docs/4.5/getting-started/introduction/)
- [HTML Living Spec](https://html.spec.whatwg.org/)
