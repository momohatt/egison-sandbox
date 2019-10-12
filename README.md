# Gröbner basis in Egison

## How to run Buchberger's algorithm
```
$ egison -l formula.egi
> (show-poly f1)
"x^2 y + -x^2"
> (show-poly f2)
"x y^2 + -y^2"
> (map show-poly (buchberger {f1 f2}))
...
{"x^3 + -x^2" "-x^2 + y^2" "x^2 y + -x^2"}
```

## Reference
* Franz Baader and Tobias Nipkow. "Term Rewriting and All That". Cambridge university press, 1999.
