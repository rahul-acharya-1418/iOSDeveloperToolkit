- Remove `.DS_Store` File from every where in your project
```
find . -name .DS_Store -print0 | xargs -0 git rm -f --ignore-unmatch
```
