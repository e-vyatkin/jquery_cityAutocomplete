# jquery.cityAutocomplete
City autocomplete dropdown

## How to Use?

City autocomplete depends on jquery and google maps js api:

```
<link rel="stylesheet" type="text/css" href="city-autocomplete.min.css"/>
<script type="text/javascript" src="//maps.googleapis.com/maps/api/js?key=API_KEY&libraries=places&language=en"></script>
<script src="jquery.js" type="text/javascript"></script>
<script src="jquery.city-autocomplete.min.js" type="text/javascript"></script>
```

Change API_KEY to your Google API KEY.
[https://developers.google.com/maps/documentation/javascript/get-api-key](Get API Key)

Create input:

```
<input id="city" name="city" autocomplete="off">
```

then

```
$('input#city').cityAutocomplete(options);
```

Possible options:  
* ```show_state``` - boolean, shows state in dropdown, default - ```false```
* ```show_country``` - boolean, shows country in dropdown, default - ```false```

You can set data-country attribute for input to search cities only for selected country:

```
<input id="city" name="city" autocomplete="off" data-country="ru">
```
