# Pine-Strategy-RSI2
# Pinescript version = 4
Read the docs for help v4 of Pinescript only!!

Please copy the code from main and put it in Pine-editor in tradingview!
https://www.tradingview.com/pine-script-docs/en/v4/index.html

This is Pinescript Strategy Code for RSI Algo

SomeThings important to know about Pinescript:

-> Pinescript has 5 versions, no version is compatible with other (mostly).
-> The script is ran once after every candle close, it's like a loop.
-> Variable declaration has different scopes. This differs a var declared in and out of an if-else, loop etc.

Controversials (I am not sure, check the docs for clarification):

-> Declaring a variable outside of an if-else or loop, and trying to change its value inside the if or loop can have unknown consequences like creating
2 variables with same name.
-> you can't declare a var without assigning a value, but the invisible loop after every candle replace this value after every iteration setting it to assigned value. Hence, we can't change its value according to our calculatiions because it will be resetted by the loop. (There is a way to get around this using ":=" instead of "=" but I am not sure so check the docs for v4 pinescript)
