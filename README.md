# Overview

This is a repo to help you practice diffing!


## Instructions

To get started:

1. Fork this repo
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
diff --git a/README.md b/README.md
index 6c6f7e3..f7b3b3e 100644
--- a/README.md
+++ b/README.md
@@ -1,10 +1,10 @@
 # Overview

 This is a repo to help you practice diffing!
 + This is a new line
 - This is a line that was removed

## Instructions
 ```

