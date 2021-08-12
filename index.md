<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.2.0/styles/devibeans.min.css">
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.2.0/highlight.min.js"></script>
<script>
elmnt = document.getElementById("included");
xhttp = new XMLHttpRequest();
xhttp.onreadystatechange = function() {
  if (this.readyState == 4) {
    if (this.status == 200) {elmnt.innerHTML = this.responseText;}
    if (this.status == 404) {elmnt.innerHTML = "Page not found.";}
    }
}
xhttp.open("GET",'include.html', true);
xhttp.send();
</script>
<div id="included"></div>
<h1>test test</h1>
<p>test text</p>
<pre class="hljs highlight language-js"><code>
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}</code></pre>

<script>hljs.highlightAll();</script>
