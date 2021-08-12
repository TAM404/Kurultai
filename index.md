<script src="https://code.jquery.com/jquery-3.6.0.slim.min.js" integrity="sha256-u7e5khyithlIdTpu22PHhENmPcRdFiHRjhAuHcs05RI=" crossorigin="anonymous"></script>
<div class="included" src="styles.html"></div>
<h1>test 14 test</h1>
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
