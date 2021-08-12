<h1>test test</h1>
<p>test text</p>
<pre class="hljs highlight language-js"><code>
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}</code></pre>


<div class="included" src="included.html"></div>
<script>
elmnts = document.getElementsByClassName("included");
for (index = 0; index < elmnts.length; index++) {
     elmnt= elmnts[index];                             
     xhttp = new XMLHttpRequest();
     xhttp.onreadystatechange = function() {
        if (this.readyState == 4) {
            if (this.status == 200) {elmnt.innerHTML = this.responseText;}
            if (this.status == 404) {elmnt.innerHTML = "Page not found.";}
        }
    }
    xhttp.open("GET",elmnt.getAttribute("src"), true);
    xhttp.send();                                   
}
</script>
