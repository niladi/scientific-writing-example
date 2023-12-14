# scientific-writing-example
This is an example project, where it derives a support structure for writing scientic articles with GitHub Actions. This specific repository holds the source files for the texts.

## Feature
* Actions to Validate LaTex
* Automated Build of PDF releases when new Tags are setted
* On every Push set new latest preview release
* Using submodule vor media (which enables buildung of for example draw.io files automatically on push further: https://github.com/niladi/scientfic-media-example -> Comment: since VS-Code aswell as github supports *.drawio.png or *.drawio.svg files it is not necessary to use this anymore ... to delete this follow ![Delete Submodule](#delete-submodule)

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
