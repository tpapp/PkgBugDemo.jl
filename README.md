# PkgBugDemo

Demo a bug in Pkg.

```julia
pkg> dev https://github.com/tpapp/PkgBugDemo.jl
pkg> activate ~/.julia/dev/PkgBugDemo
pkg> add Parameters
pkg> rm Parameters
shell> git diff
diff --git a/Project.toml b/Project.toml
index 6609aa4..4ae035b 100644
--- a/Project.toml
+++ b/Project.toml
@@ -3,10 +3,5 @@ uuid = "b4ea9972-f880-5dc1-8aaf-ab4ea81b0c3f"
 authors = ["Tamas K. Papp <tkpapp@gmail.com>"]
 version = "0.1.0"

-[deps]
-
 [extras]
 Test = "8dfed614-e22c-5e08-85e1-65c5234f0b40"
-
-[targets]
-test = ["Test"]
```
