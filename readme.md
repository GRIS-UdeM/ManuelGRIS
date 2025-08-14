# Builds for the SpatGRIS manuals

## todo:
Figure out the exact dependencies for pandoc/latex

## how to use

### dependencies

- xonsh (`sudo apt install xonsh`)
- inkscape (for emf image files) (`sudo apt install inkscape`)
- pandoc + a whole bunch of latex stuff (good luck, try installing stuff until it stops complaining)

### convert docx to md

If you have a new docx version of the manual, you can do the whole conversion to `.md`, complete with image extraction and `.emf` conversion by running `scripts/make-md-sources-from-docx.xonsh`.

This will create a .md file for the english and french version of the manual. You'll have to change the path of the docx files in the `do_it` calls of the `make-md-sources-from-docx.xonsh` file.

### make pdfs and htmls

Once you have md files or if you have modified the md and media files, run `scripts/make-outputs.xonsh`
