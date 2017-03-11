<h1>**Forecast App**</h1>

<p>This app shows the current weather conditions and a static picture of the
selected city.</p>
<p>The Conditions are</p>
<ul>
<li>Temperature</li>
<li>Wind speed and Direction</li>
<li>Dew Point</li>
</ul>

```
     wsc.getLatLonForSelected = function(){
                GoogleGeolocationService.geoLocate(wsc.selected_city)
                    .then(function(res){
                        wsc.selected_lat = res.data.results[0].geometry.location.lat;
                        wsc.selected_lon = res.data.results[0].geometry.location.lng;
                        
                        wsc.selected_city.lat = wsc.selected_lat;
                        wsc.selected_city.lon = wsc.selected_lon;
                        ```


	
	
	
