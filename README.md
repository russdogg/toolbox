Russdesigns Toolbox » Version 0.1
=================================

This is my first attempt at putting together a javascript toolkit all in one place.


Email validation:
-----------------

	function checkMail(email){
	var filter  = /^([a-zA-Z0-9_\.\-])+\@(([a-zA-Z0-9\-])+\.)+([a-zA-Z0-9]{2,4})+$/;
		if (filter.test(email)) {
		return true;
		}
		return false;
	}    

iPhone style orientation change detection:
------------------------------------------

	window.addEventListener('load', setOrientation, false);
	window.addEventListener('orientationchange', setOrientation, false);
	
	function setOrientation() {
		var orient = Math.abs(window.orientation) === 90 ? 'landscape' : 'portrait';
		var cl = document.body.className;
		cl = cl.replace(/portrait|landscape/, orient);
		document.body.className = cl;
	}

Some people seem to like definition lists

<dl>
  <dt>Lower cost</dt>
  <dd>The new version of this product costs significantly less than the previous one!</dd>
  <dt>Easier to use</dt>
  <dd>We've changed the product so that it's much easier to use!</dd>
</dl>


Table for two
-------------

<table>
  <tr>
    <th>ID</th><th>Name</th><th>Rank</th>
  </tr>
  <tr>
    <td>1</td><td>Tom Preston-Werner</td><td>Awesome</td>
  </tr>
  <tr>
    <td>2</td><td>Albert Einstein</td><td>Nearly as awesome</td>
  </tr>
</table>

Crazy linking action
--------------------

I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"