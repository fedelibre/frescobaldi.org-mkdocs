# Releases

## Changes in current master

Requirement changes:

  - Frescobaldi now requires Python3.3+

New features:

  - New "Document Fonts" dialog supporting text and music fonts
    and providing a font sample previewer
  - Possibility to load external extensions
  - New "First System Only" option in Custom Engrave
  - Goto Line command (#927, feature request #676)
  - Rename file command (#1057, feature request #980)

Bug fixes:

  - fixed #895 seeking in MIDI player during playing stops sound
  - fixed #768, now paper orientation is properly handled in New Score Wizard
  - fixed #705, discrepancy of LilyPond vs. system version of GhostScript
    on Linux (#926)
  - fixed #1094, includepaths on Windows (#1095)
  - fixed #1121, NameError: name 'widgets' is not defined

Improvements:

  - Smarter behaviour of the autocompletion popup (#918, #922)
  - New command File->Rename/Move... (#980)
  - Sessions can be grouped in the Sessions menu
  - Show absolute path of include files in tooltip (#941)
  - Restructure Tools Menu (#1080)
  - File Open toolbar button shows recent files menu on long click

Internals:

  - Multithreaded Job Queue preparing multicore support (#1103)
  - Rewrite code handling external processes/jobs (#1100)


## Changes in 3.0.0 -- 2017/02/17

Requirement changes:

  - Frescobaldi now requires Python3.2+, Qt5, PyQt5, python-poppler-qt5

New features:

  - Zoom with pinch gesture in Music View, contributed by David Rydh
  - An option (enabled by default) to move the cursor to the end of the line
    when PageDown is pressed on the last line, and to move the cursor to the
    start of the first line if PageUp is pressed on the first line

Improvements:

  - Retina display support in Music View, contributed by David Rydh
