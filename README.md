# ISO3166

This unit allows you to obtain a name of a country and it's emoji flag based on a iso3166 code. This code can one of the following:

* alfa - 2 digits
* alfa - 3 digits
* numeric - 3 digits

This unit allows you to convert between formats as well.

* alfa2 → alfa3
* alfa2 → numeric
* alfa3 → alfa2
* alfa3 → numeric
* numeric → alfa2
* numeric → alfa3

To obtain a country name based on its 2 digit alfanumerical code you may do:

```python
#Import the unit
import iso3166
#Instantiate the class
myCountry = iso3166.ISO3166()
#Print the country name (not UN conform. I prettyfied it)
print( myCountry.get_alfa2( 'ES' )[0] )
#Not print the flag. Bare in mind that your terminal has to be able to print it!
print( myCountry.get_alfa2( 'ES' )[1] )

```

This will print out:
```
Spain
🇪🇸
````

## Available methods:
| Method | Parameter(s) | Returns |
|:-------|:----------:|--------:|
| **get_alfa2( code )** | The country code | A list containing: [0] Country Name, [1]  Country Flag
| **get_alfa3( code )** | The country code | A list containing: [0] Country Name, [1] Country Flag
| **get_numeric( code )** | The country code | A list containing: [0] Country Name, [1] Country Flag
| **convert_alfa2_alfa3( code )** | The country code | The alfa3 equivalent of code |
| **convert_alfa2_numeric( code )** | The country code | The numeric equivalent of code |
| **convert_alfa3_alfa2( code )** | The country code | The alfa2 equivalent of code |
| **convert_alfa3_numeric( code )** | The country code | The numeric equivalent of code |
| **convert_numeric_alfa2( code )** | The country code | The alfa2 equivalent of code |
| **convert_numeric_alfa3( code )** | The country code | The alfa3 equivalent of code |
