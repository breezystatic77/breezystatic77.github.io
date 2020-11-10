# Coding

In addition to standard Markdown profiles, Thespian supports writing profiles in custom HTML, CSS, and Javascript.

Activate the "HTML Mode" switch on your character's profile to begin coding.

?> This section assumes you know how to code in HTML / CSS / Javascript. If you're interested, [Codecademy](https://www.codecademy.com/learn/learn-html) is a great place to start.

## Technical Stuff

Your profile runs inside of a sandboxed iframe for security. Within that sandbox, the full Javascript library is available.

Here are some examples of simple profiles using all 3 languages.

```html
<style>
 h1 {
  color: tomato;
 }
</style>

<h1>This text is a different format than normal.</h1>

<script type="text/javascript">
 alert("Wow, an alert!");
</script>
```

A profile that imports the external library [jQuery](https://jquery.com/)

```html
<h1>This text is unedited</h1>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script type="text/javascript">
 $("h1").text("this text is edited by jQuery");
 $("h1").click(function() {
  $("h1").text("You clicked it!");
 });
</script>
```

A profile that imports the external library [Vue](https://vuejs.org/)

```html
<div id="app">
 {{ message }}
</div>

<script src="https://cdn.jsdelivr.net/npm/vue@2"></script>
<script type="text/javascript">
 var app = new Vue({
  el: '#app',
  data: {
   message: 'This text is created by Vue'
  }
 });
</script>
```
