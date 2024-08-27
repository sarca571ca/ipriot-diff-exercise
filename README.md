# Overview

This is a repo to help you practice diffing!


## Instructions

To get started:

1. Fork this repo.
⚠️ IMPORTANT: Fork all branches. Not just `main`
2. Clone your forked repo:
```bash
git clone <your-forked-repo-url>
```

Follow these instructions carefully.

## Diffing

A diff is a speciifc file format that tells you the difference between lines in a file and optionally words on that line. It contains enough context to make sense to humans and enough information to allow a machine to apply a difference to a set of files such that:

$$
A = B \circ \text{Apply}(\text{Diff}(A, B))
$$
That is, the difference between A and B can allow A to be transformed into B and vice versa using a function that **applies** said difference.

Let's now look at an example diff:

```diff
diff --git a/README.md b/README.md ①
index 7f35690..14cf26a 100644 ②
--- a/README.md ③
+++ b/README.md
@@ -8,9 +8,12 @@ ④
This is a repo to help you practice diffing!
 To get started:

 1. Fork this repo ⑤
-2. Clone your forked repo ⑥
+2. Clone your forked repo:
+```bash
+git clone <your-forked-repo-url>
+```

-Follow these instructions c.a.r.e.f.u.l.l.y. ⑦
+Follow these instructions carefully.
```

Fill in what each of the elements of the diff mean (if you are not sure just guess!):
**①**:
> Insert your answer here

**②**:
> Insert your answer here

**③**:
> Insert your answer here

**④**:
> Insert your answer here

**⑤**:
> Insert your answer here

**⑥**:
> Insert your answer here

**⑦**:
> Insert your answer here


Notice that the diff above only showed different **lines** in the file. This is the default behavior of the `diff` command. However, you can also show the difference between words in a line by using the `-w` flag. For example:

 