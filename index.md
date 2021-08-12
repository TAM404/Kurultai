<div class="included" src="include.html"></div>

<h1>test 2 test</h1>
<p>test text</p>
<pre class="hljs highlight language-js"><code>
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}</code></pre>


<div class="included" src="styles.html"></div>
<div class="included" src="include.html"></div>
<script>
async function httpstuff(elmnt){
       xhttp = new XMLHttpRequest();
     async xhttp.onreadystatechange = function() {
        if (this.readyState == 4) {
            if (this.status == 200) {elmnt.innerHTML = this.responseText;}
            if (this.status == 404) {elmnt.innerHTML = "Page not found.";}
        }
    }
    xhttp.open("GET",elmnt.getAttribute("src"), true);
    xhttp.send();   
  }
elmnts = document.getElementsByClassName("included");
for (index = 0; index < elmnts.length; index++) {
     elmnt= elmnts[index];
     httpstuff(elmnt);
}
</script>
