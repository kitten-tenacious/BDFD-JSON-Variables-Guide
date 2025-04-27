# BDFD-JSON-Variables-Guide
A brief and understanding Guide about how JSON variables can be done in BDFD for storing huge amounts of variables in a single variable.

In this Guide, we'll be covering about JSON Functions and it's relatives (obviously not all functions), which can help you shrink the size of your variable counts alot and store much stuff inside a single variable.

## JSON Functions

- [$jsonParse](#jsonparse)
- [$jsonSet](#jsonset)
- [$jsonSetString]($jsonsetstring)
- [$jsonStringify](#jsonstringify)
- [$jsonUnset](#jsonunset)

---

### $jsonParse

This is the very beginning of JSON Variables, with starting off using `$jsonParse`. This function is extremely important when reading this guide, because we'll be using this function in literally every single code.
Let's see how this function works.

```codeblock
$jsonParse[{
"name": "value"
}]
```
This is how `$jsonParse` works. `$jsonParse` is a function that takes a block of text (in JSON format) and turns it into a format your bot can easily understand and use, like picking specific values from it.
It parses a string into an object. A text that is inside quotes (") are called **Strings**. So, to retrieve the value of "name" in this case, we'll retrieve it using the help of `$json`.


```codeblock
$jsonParse[{
"name": "value"
}]

Value of "name": $json[name]
```

Now the code will return the value of "name", which is "value".
