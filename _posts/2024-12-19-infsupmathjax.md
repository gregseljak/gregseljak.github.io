---
layout: post
title: Lim Sup/Inf notation
subtitle: (Hello World for MathJax)
mathjax: true
date: 2024-12-19
tags: [math, test]
author: Greg
---
<br><br><br><br>

### \\(\overline{\lim}A_n\\) vs \\(\underline{\lim}A_n\\)

When it comes to limits of sets, I've always had a hard time keeping the notation of \\(\overline{\lim}A_n\\) and \\(\underline{\lim}A_n\\) straight in my head. Was it cup-cap or cap-cup? To be sure, it's

\\[\underline{\lim}A_n=\cup_{n\geq 1}\cap_{j\geq n}A_j\\]

\\[\overline{\lim}A_n=\cap_{n\geq 1}\cup_{j\geq n}A_j\\]

On the other hand, the lim sup/inf of functions (or sequences) has an obvious interpretation and are easy to remember. The intuitive definitions of \\(\overline{\lim}x_n\\) and \\(\underline{\lim}x_n\\) for me were:

- \\(\underline{\lim}x_n=\underline{x}\\) is the smallest limit point such that there exists a subsequence \\(\phi:\mathbb{N}\rightarrow\mathbb{N}\\) with \\(\lim x_{\phi(n)}=\underline{x}\\)
<br>

- Equivalently (but less intuitively), \\(\underline{\lim}x_n=\lim_{n\rightarrow \infty}\left(\inf_{m\geq n}x_m\right)\\)
<br>

Then the definitions for the \\(\overline{\lim}x_{n}\\) are just changed to be sup instead of inf. Once you see a visualization, it's impossible to get these confused. Here's a simple sequence \\(x_n\\) that does not converge, but has pretty clearly:<br>\\(\underline{x}=-1,\text{ and }\,\mspace{3mu}\overline{x}=1\\)

![limsupinf_sequence](/assets/img/2024-12-19-infsupmathjax.png)

The limit definitions for sets makes sense, but it's not clear how these are at all related to the definitions for sequences. The two concepts share notation because they are in some ways analogous to each other, but there isn't a really precise correspondence between the two. It's true that for positive measure \\(\mu\\) we'll have

\\[\mu\left(\underline{\lim}A_n\right)\leq\mu\left(\overline{\lim}A_n\right)\\]
\\[\underline{\lim}x_n\leq\overline{\lim}x_n\\]

The following "exercise" shows an example relationship that can be used as a mnemonic. It's not terribly profound, but I wish I'd thought of it when taking Real Analysis. Not a bad quiz question for an intro course, maybe.

**Exercise (trivial):** 
\\[\text{Let }\{x_n\}\text{ be an infinite sequence in }\mathbb{R}\\]
\\[\text{Let }A_n=(-\infty,x_n]\\]

**Question:** Find the inf/sup limits of \\(A_n\\) in terms of the inf/sup limits of \\(x_n\\).
<br>
<br><br>
I also like the idea of the inf/sup limits of \\(A_n\\) as articulated in plain language:

- \\(\overline{\lim}A_n\\): The set of things that are always approaching at some future time
<br>
- \\(\underline{\lim}A_n\\): The set of things that eventually happen every time
<br>
<br>

That seems nice, but subsequent logic is totally unwieldly. How do you explain the fact that a singular limit exists iff these two sets equal each other? "When everything that will eventually happen is always happening, nothing will ever change". It's not exactly Shakespearean. But that's math.