# Builds for the SpatGRIS manuals

## dependencies

- cargo/rust
- mdbook (`cargo install mdbook`)

## Editing the manuals

- Go into `sources/spatgris-man-en/src` and `sources/spatgris-man-fr/src`
- Edit the relevant chapters
- In the mdbook folder (`sources/spatgris-man-en` or `sources/spatgris-man-fr`) run `mdbook build`
- You can run `mdbook serve` to have a webserver where you can see the result of your edits live as soon as you save a file.

## todo:

### content

- Make a more beautiful landing page
- Update numbering in md files to match mdbook autonumbering
- Update english doc to match french doc (and vice-versa)
- Update images
- Add links to issue trackers
- Add sat developpers, testers, project managers credits
