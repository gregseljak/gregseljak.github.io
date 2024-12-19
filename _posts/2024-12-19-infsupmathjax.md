---
layout: post
title: Lim Sup/Inf notation
subtitle: Hello World
mathjax: true
date: 2024-12-19
tags: [math, test]
author: Greg
---







### MathJax Test Post

When it comes to limits of sets, I've always had a hard time keeping \\(\overline{\lim}A_n\\) and \\(\underline{\lim}A_n\\) straight in my head.
On the other hand, the lim sup/inf of functions (or sequences) has an obvious interpretation. I would never mix up \\(\overline{\lim}x_n\\) and \\(\underline{\lim}x_n\\). In school I learned that

- \\(\underline{\lim}x_n=x^-\\) is the smallest limit point such that there exists a subsequence \\(\phi(n)\\) with \\(\lim x_{\phi(n)}=x^-\\)
- likewise for \\(\overline{\lim}x_n\\)

On the other hand,

\\[\underline{\lim}A_n=\cup_{n\geq 1}\cap_{j\geq n}A_j\\]

\\[\overline{\lim}A_n=\cap_{n\geq 1}\cup_{j\geq n}A_j\\]

I knew that the two concepts shared notation because they were in some ways analogous to each other, but I never really thought about the precise
correspondence between the two. It's more of a mnemonic than a really profound finding, but maybe others can use it too.

\\[\text{Let }\{x_n\}\text{ be an infinite sequence in }\mathbb{R}\\]
\\[\text{Let }A_n=(-\infty,x_n]\\]

Now find the inf/sup limits of \\(A_n\\) in terms of the inf/sup limits of \\(x_n\\).

I also like the idea of the inf/sup limits of \\(A_n\\) as articulated in plain language:
- \\(\underline{\lim}A_n\\): The set of things that eventually always happen
- \\(\overline{\lim}A_n\\): The set of things that are always approaching
That seems nice, but the conclusion is totally unwieldly. "When everything that will eventually happen is always happening, nothing will ever change". It is not exactly Shakespearean. But that's math.