Running ``stylefmt`` via npm scripts ignores files but running that same command directly works as expected

Output:

```
stylefmt-recursive ➜ npm run fix

> stylefmt-recursive@1.0.0 fix /Users/chris/github/stylefmt-recursive
> stylefmt --config .stylelintrc.js --recursive src/**/*.css

src/dir1/dir1.css

1 files are formatted.


stylefmt-recursive ➜ stylefmt --config .stylelintrc.js --recursive src/**/*.css
src/dir1/dir2/dir2.css, src/src.css

2 files are formatted.


stylefmt-recursive ➜ npm -v
3.10.8
stylefmt-recursive ➜ node -v
v6.9.1
```