**HTTP Request: `Invoke-WebRequest`** is used to send an HTTP request to the 
specified URI. The `-Headers` parameter includes the custom headers.

**JSON Parsing:** The response content is converted from JSON using 
`ConvertFrom-Json`. To pretty-print the output, it's then 
piped into `ConvertTo-Json`.

**Check Response:** The script checks if the `ok` property in the JSON response 
is `true`. If not, it prints "Error" and exits with status 1.