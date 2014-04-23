#Arcnet Simple Format Plugin
A jQuery Plugin to make formats on form fields and HTML elements with some formats defined.

##Compatibility

Jquery Arcnet Simple Format Plugin has been tested with jQuery 1.7+ on all major browsers:

* Firefox 2+ (Win, Mac, Linux);
* IE7+ (Win);
* Chrome 6+ (Win, Mac, Linux, Android, iPhone);
* Safari 3.2+ (Win, Mac, iPhone);
* Opera 8+ (Win, Mac, Linux, Android, iPhone).


##Basic Usage Examples
###Mask using data-format attribute
To get your format applied with the data-format attribute just use it in your input field, when you unfocus(on-blur)the input the magic happens and the input is formatted.

```bash
<input type="text" data-format="toupper" /><br>
//=>all letters typed will stay uppercase

<input type="text" data-format="tolower" /><br>
//=>all letters typed will stay lowerrcase

<input type="text" data-format="firstupper" /><br>
//=>the first word typed will stay with the first letter in uppercase

<input type="text" data-format="allfirstsupper" /><br>
//=>all letters typed will stay with the first letter in uppercase

<input type="text" data-format="cnpj" /><br>
//=>The sequence of numbers typed will stay format as a cnpj format

<input type="text" data-format="cnpjstripe" /><br>
//the cnpj format typed will stay with only numbers, removing the special characters

<input type="text" data-format="cpf" /><br>
//=>The sequence of numbers typed will stay format as a cpf format

<input type="text" data-format="cpfstripe" /><br>
//the cpf format typed will stay with only numbers, removing the special characters

<input type="text" data-format="toCurrency" /><br>
//the string typed in the input will be converted for currency

<input type="text" data-format="militodate" /><br>
//the millisecods typel will be converted in date like DD/MM/YY
```

###Mask using data-format-realtime attribute
Is the same of data-format, the only difference is that as you type the word is formatted
```bash
<input type="text" data-format-realtime="toupper" /><br>
//=>all letters typed will stay uppercase instantly

<input type="text" data-format-realtime="tolower" /><br>
//=>all letters typed will stay lowerrcase instantly

<input type="text" data-format-realtime="firstupper" /><br>
//=>the first word typed will stay with the first letter in uppercase instantly

<input type="text" data-format-realtime="toCurrency" /><br>
//=>the string typed in the input will be converted for currency instantly
```

##Using the methods
```bash
z.cnpjStrip("91.576.861/0001-78")
//=>91576861000178

z.cnpjFormat(91576861000178)
//=>91.576.861/0001-78

z.cpfStrip("445.460.157-71")
//=>44546015771

z.cpfFormat(44546015771)
//=>445.460.157-71
```

#License
Created by Weslley Neri on 2014-02-25 - https://github.com/weslley39

 Copyright (c) 2014 Arcnet - Automação Comercial (http://arcnet.com.br/)

 The MIT License (http://www.opensource.org/licenses/mit-license.php)

 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following
 conditions:

 The above copyright notice and this permission notice shall be
 included in all copies or substantial portions of the Software.

 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
 OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
