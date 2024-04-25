#book 

**R**ip**G**rep is recursive search for line with given regex pattern in rust regex convention. By default it respect hidden files, .gitignore and skips binary files.

## Example
> [[rg]] "\[ab\]\[cd\]"

It will print all lines group by files, which contains pattern `[ab][cd]`, so one letter is either `a` or `b`, followed by either `c` and `c`.