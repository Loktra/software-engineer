## Task

Write code to find a 9 letter string of characters that contains only letters from

`acdegilmnoprstuw`

such that the hash(the_string) is

`930846109532517`

if hash is defined by the following pseudo-code:

```
Int64 hash (String s) {
    Int64 h = 7
    String letters = "acdegilmnoprstuw"
    for(Int32 i = 0; i < s.length; i++) {
        h = (h * 37 + letters.indexOf(s[i]))
    }
    return h
}
```

For example, if we were trying to find the 7 letter string where `hash(the_string)` was `680131659347`, the answer would be "leepadg".
