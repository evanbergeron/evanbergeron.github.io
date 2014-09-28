---
layout: post
title: Markov Text and Variations
---

I recently wrote a small program that generates random text from an arbitrary number of sample texts.

Here's how it works:

Your text is a list of words. From this list of words, you create a list of sequences of adjacent words, or snippets, or words.

If your text was "I never cared for cherries," you list of snippets might become

```py
[["I", "never", "cared"],
["never", "cared", "for"],
["cared", "for", "cherries"]]
```

You can change the length of these snippets, if you like.

From this list of snippets, choose one of the snippets as the start of your random text.
