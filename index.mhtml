<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  <meta http-equiv="Content-Style-Type" content="text/css">
  <title></title>
  <meta name="Generator" content="Cocoa HTML Writer">
  <meta name="CocoaVersion" content="1504.83">
  <style type="text/css">
    p.p1 {margin: 0.0px 0.0px 0.0px 0.0px; font: 12.0px Helvetica}
    p.p2 {margin: 0.0px 0.0px 0.0px 0.0px; font: 12.0px Helvetica; min-height: 14.0px}
  </style>
</head>
<body>
<p class="p1">&lt;!DOCTYPE html&gt;</p>
<p class="p1">&lt;html&gt;</p>
<p class="p1">&lt;head&gt;</p>
<p class="p1">&lt;meta name="viewport"/&gt;</p>
<p class="p1">&lt;title&gt;astraptes_fulgerator_complex_sample_data - Google Fusion Tables&lt;/title&gt;</p>
<p class="p1">&lt;style type="text/css"&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>html, body, #googft-mapCanvas {</p>
<p class="p1"><span class="Apple-converted-space">    </span>height: 300px;</p>
<p class="p1"><span class="Apple-converted-space">    </span>margin: 0;</p>
<p class="p1"><span class="Apple-converted-space">    </span>padding: 0;</p>
<p class="p1"><span class="Apple-converted-space">    </span>width: 500px;</p>
<p class="p1"><span class="Apple-converted-space">  </span>}</p>
<p class="p1">&lt;/style&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;script type="text/javascript" src="https://maps.google.com/maps/api/js?v=3&amp;amp;libraries=visualization"&gt;&lt;/script&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;script type="text/javascript"&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>if (window.location.protocol == "file:") {</p>
<p class="p1"><span class="Apple-converted-space">    </span>alert('This script only works when loaded from a web server,' +</p>
<p class="p1"><span class="Apple-converted-space">        </span>' not from a file on your computer.');</p>
<p class="p1"><span class="Apple-converted-space">  </span>}</p>
<p class="p1"><span class="Apple-converted-space">  </span>function ftOnLoadClientApi() {</p>
<p class="p1"><span class="Apple-converted-space">  </span>}</p>
<p class="p1">&lt;/script&gt;</p>
<p class="p1">&lt;script type="text/javascript" src="https://apis.google.com/js/client.js?onload=ftOnLoadClientApi"&gt;</p>
<p class="p1">&lt;/script&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;script type="text/javascript"&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>var map;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>function loadApi() {</p>
<p class="p1"><span class="Apple-converted-space">    </span>gapi.client.load('fusiontables', 'v1', initialize);</p>
<p class="p1"><span class="Apple-converted-space">  </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>function initialize() {</p>
<p class="p1"><span class="Apple-converted-space">    </span>var isMobile = (navigator.userAgent.toLowerCase().indexOf('android') &gt; -1) ||</p>
<p class="p1"><span class="Apple-converted-space">      </span>(navigator.userAgent.match(/(iPod|iPhone|iPad|BlackBerry|Windows Phone|iemobile)/));</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (isMobile) {</p>
<p class="p1"><span class="Apple-converted-space">      </span>var viewport = document.querySelector("meta[name=viewport]");</p>
<p class="p1"><span class="Apple-converted-space">      </span>viewport.setAttribute('content', 'initial-scale=1.0, user-scalable=no');</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1"><span class="Apple-converted-space">    </span>var mapDiv = document.getElementById('googft-mapCanvas');</p>
<p class="p1"><span class="Apple-converted-space">    </span>mapDiv.style.width = isMobile ? '100%' : '500px';</p>
<p class="p1"><span class="Apple-converted-space">    </span>mapDiv.style.height = isMobile ? '100%' : '300px';</p>
<p class="p1"><span class="Apple-converted-space">    </span>map = new google.maps.Map(mapDiv, {</p>
<p class="p1"><span class="Apple-converted-space">      </span>center: new google.maps.LatLng(10.882753836500974, -85.35149247558599),</p>
<p class="p1"><span class="Apple-converted-space">      </span>zoom: 11,</p>
<p class="p1"><span class="Apple-converted-space">      </span>mapTypeId: google.maps.MapTypeId.ROADMAP</p>
<p class="p1"><span class="Apple-converted-space">    </span>});</p>
<p class="p1"><span class="Apple-converted-space">    </span>var query = 'select col12, col13 from 1KeaOABzhzWg7CkOZn7UskkoqpNTRYQpOTbbZWkr_ limit 1000';</p>
<p class="p1"><span class="Apple-converted-space">    </span>var request = gapi.client.fusiontables.query.sqlGet({ sql: query });</p>
<p class="p1"><span class="Apple-converted-space">    </span>request.execute(function(response) {</p>
<p class="p1"><span class="Apple-converted-space">      </span>onDataFetched(response);</p>
<p class="p1"><span class="Apple-converted-space">    </span>});</p>
<p class="p1"><span class="Apple-converted-space">  </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>function onDataFetched(response) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (response.error) {</p>
<p class="p1"><span class="Apple-converted-space">      </span>alert('Unable to fetch data. ' + response.error.message +</p>
<p class="p1"><span class="Apple-converted-space">          </span>' (' + response.error.code + ')');</p>
<p class="p1"><span class="Apple-converted-space">    </span>} else {</p>
<p class="p1"><span class="Apple-converted-space">      </span>drawHeatmap(extractLocations(response.rows));</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1"><span class="Apple-converted-space">  </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>function extractLocations(rows) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>var locations = [];</p>
<p class="p1"><span class="Apple-converted-space">    </span>for (var i = 0; i &lt; rows.length; ++i) {</p>
<p class="p1"><span class="Apple-converted-space">      </span>var row = rows[i];</p>
<p class="p1"><span class="Apple-converted-space">      </span>if (row[0]) {</p>
<p class="p1"><span class="Apple-converted-space">        </span>var lat = row[0];</p>
<p class="p1"><span class="Apple-converted-space">        </span>var lng = row[1];</p>
<p class="p1"><span class="Apple-converted-space">        </span>if (lat &amp;&amp; lng &amp;&amp; !isNaN(lat) &amp;&amp; !isNaN(lng)) {</p>
<p class="p1"><span class="Apple-converted-space">          </span>var latLng = new google.maps.LatLng(lat, lng);</p>
<p class="p1"><span class="Apple-converted-space">          </span>locations.push(latLng);</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">      </span>}</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1"><span class="Apple-converted-space">    </span>return locations;</p>
<p class="p1"><span class="Apple-converted-space">  </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>function drawHeatmap(locations) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>var heatmap = new google.maps.visualization.HeatmapLayer({</p>
<p class="p1"><span class="Apple-converted-space">       </span>dissipating: true,</p>
<p class="p1"><span class="Apple-converted-space">       </span>gradient: [</p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(102,255,0,0)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(147,255,0,1)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(193,255,0,1)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(238,255,0,1)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(244,227,0,1)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(244,227,0,1)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(249,198,0,1)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(255,170,0,1)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(255,113,0,1)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(255,57,0,1)',<span class="Apple-converted-space"> </span></p>
<p class="p1"><span class="Apple-converted-space">         </span>'rgba(255,0,0,1)'</p>
<p class="p1"><span class="Apple-converted-space">       </span>],</p>
<p class="p1"><span class="Apple-converted-space">       </span>opacity: 0.51,</p>
<p class="p1"><span class="Apple-converted-space">       </span>radius: 30,</p>
<p class="p1"><span class="Apple-converted-space">       </span>data: locations</p>
<p class="p1"><span class="Apple-converted-space">    </span>});</p>
<p class="p1"><span class="Apple-converted-space">    </span>heatmap.setMap(map);</p>
<p class="p1"><span class="Apple-converted-space">  </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>google.maps.event.addDomListener(window, 'load', loadApi);</p>
<p class="p1">&lt;/script&gt;</p>
<p class="p1">&lt;/head&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;body&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;div id="googft-mapCanvas"&gt;&lt;/div&gt;</p>
<p class="p1">&lt;/body&gt;</p>
<p class="p1">&lt;/html&gt;</p>
</body>
</html>
