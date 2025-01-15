# FontMake issue

## Reproduction

First, generate a UFO+designspace:

```
glyphs2ufo '/Users/stephennixon/type-repos/00-issue-reports/test-fontmake-rvrn/01-src/ExampleSans.glyphs' --output-dir 02-glyphs2ufo
```

Then, build fonts:

```
fontmake -o variable -m '/Users/stephennixon/type-repos/00-issue-reports/test-fontmake-rvrn/02-glyphs2ufo/ExampleSans.designspace' --output-dir 03-fonts
fontmake -o otf -i -m '/Users/stephennixon/type-repos/00-issue-reports/test-fontmake-rvrn/02-glyphs2ufo/ExampleSans.designspace' --output-dir 03-fonts
```