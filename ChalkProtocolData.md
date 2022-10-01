8 bits will be dedicated to info about the data being sent
2 of those bits will be dedicated to type of data
00 will be for `get`ing data
01 will be for `give`ing data
10 and 11 are undecided and just there if we want to expand the types of data able to be sent.

The rest of the data will be JSON
The format for giving data will be
```
{
    "message": String,
    "display": Option<String>, // Display name for sender of the message
}
```
Get is not defined currently as there is no concept of history or ids for messages
