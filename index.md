<script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous"></script>
<div class="included" src="styles.html"></div>
<h1>test 16 test</h1>
<p>test text</p>
<pre class="hljs highlight language-js"><code>
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}</code></pre>

<div class="included" src="include.html"></div>
<script>
elmnts = document.getElementsByClassName("included");
for (index = 0; index < elmnts.length; index++) {
     elmnt= elmnts[index];
     $(elmnt).load(elmnt.getAttribute("src"));
}
var DOMContentLoaded_event = document.createEvent("Event")
DOMContentLoaded_event.initEvent("DOMContentLoaded", true, true)
window.document.dispatchEvent(DOMContentLoaded_event)
                                      
</script>
