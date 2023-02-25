Here are some math equations: $\frac{a^2 + b^2}{c^2} = 1$.

Here it is in double-dollar signs:
$$\frac{a^2 + b^2}{c^2} = 1$$

Here's a more complex expression, in double-dollar signs:

$$E\left[ \left( ∑_{i=1}^N \tilde w_i 2^{-q t/h_i}  \right)^{1/q} \right]$$

Next, I render this to HTML via Pandoc version 2.19.2:
```sh
pandoc -f gfm+tex_math_dollars --mathjax -s -t html5 -i README.md -o index.html
```

That HTML will be available at https://fasiha.github.io/mathjax-pandoc-accessibility

We can also convert this to MathML instead of MathJax:
```sh
pandoc -f gfm+tex_math_dollars --mathml -s -t html5 -i README.md -o index-mathml.html
```
See that: https://fasiha.github.io/mathjax-pandoc-accessibility/index-mathml.html
