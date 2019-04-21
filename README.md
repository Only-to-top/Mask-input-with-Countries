# Mask-input-with-Counties

```html
<link rel="stylesheet" href="libs/intlTelInput/css/intlTelInput.css">

<input type="tel" name="Телефон" id="phone" required>

<script src="libs/intlTelInput/js/intlTelInput.min.js"></script>

<script>
  
  // phone mask
  var input = document.querySelector("#phone");
  window.intlTelInput(input, {
    preferredCountries: ["ru", "ua", "by"],
    utilsScript: "libs/intlTelInput/js/utils.js?1549804213570",
  });
  // placeholder
  var countryData = window.intlTelInputGlobals.getCountryData(), input = document.querySelector("#phone");
  for (var i = 0; i < countryData.length; i++) { var country = countryData[i]; country.name = country.name.replace(/.+\((.+)\)/,"$1"); }
  
</script>
```
