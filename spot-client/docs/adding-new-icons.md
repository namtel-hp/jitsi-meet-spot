# Adding new font icons

The spot client uses a mix of material design icons, custom icons, and maybe other icons. To enable the various icons to be used without loading each as an image, a font is created with ligatures enabled; this allows for icons to be displayed using specified icon names instead of css classes. This is done by using icomoon.io. To update the icons with new images (SVGs):

1. Visit https://icomoon.io/app/#/select
1. Click the hamburger menu > New Project > Import Project. The file picker should display.
1. Select selection.json, which is file generated by icomoon describing the font file.
1. Load the imported project. All the icons used in the project should be displayed and selected.
1. Click Import Icons. The file picker should display.
1. Select all the desired imports and verify they have been imported.
1. Make sure all desired icons are displayed and selected.
1. Click Generate Font. All selected fonts should display.
1. Ensure ligatures is enabled ("fi" at the top of the page).
1. Find the new fonts and modify the "fi" field with the icon name that should be declared in the dom for the icon to display.
1. Click Download. This should download a zip files. Within the zip file should be a selection.json and all the font files in a fonts folder.
1. Replace the selection.json in the spot repo with the newly generated selection.json.
1. Replace all the font files with the newly generated font files.
1. Check locally that the icons display okay.
1. Commit selection.json and the font files.