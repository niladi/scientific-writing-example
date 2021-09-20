# scientific-writing-example
This is an example project, where it derives a support structure for writing scientic articles with GitHub Actions. This specific reposetory holds the source files for the texts.

## Links
The example is derived from: https://guides.nyu.edu/LaTeX/sample-document

## Delete Submodule
```
git submodule deinit scientfic-media-example
git rm scientfic-media-example
git commit-m "Removed submodule "
rm -rf .git/modules/scientfic-media-example
```

## Use this as Template
1. https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template
2. Delete Submodule
3. Create a personal-acess-token with teh acess to read repos and write releases, with the kex: `GIT_PAT`
4. Create your Latex base structure
5. Rename the main file in the `.github/workflows/main.yml`(row 22)
6. Enjoy!