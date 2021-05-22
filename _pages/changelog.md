---
layout: page
title: Changelog
include_in_header: true
---

# Release 2

## 2.1

Search Filters and Improvements:
* Filter ASCII search with RegEx and select case sensitivity
* Share search results
* Select search results in the document

Jump to Offset:
* Jump to a given hexadecimal offset
* Highlight the byte at the given index

Codepages Support:
* Select one of multiple codepages
* Support for ASCII, ISO Latin, and EBCDIC
* Select multiple syntax themes for each
* Classic HexFiend and HexDump modes

Metadata Information:
* View metadata in analysis tab
* Inspect UTI, creation date, modification date and Unix Permissions

iPadOS Cursor Support:
* Cursor snaps accurately to bytes
* Cursor snaps to byte frequencies
* Added secondary click options to many buttons

Visual Improvements:
* New app icons!
* New “Shaded of Purple” theme
* Alternating rows option
* Indicate currently open sidebar
* Change sidebar color to resemble iWork apps
* Increase sidebar width
* Removed sidebar slideover mode
* Indicated byte in frequency grid
* Changed some contrasts for accessibility
* Linked new website and mail
* Further small design tweaks

Bug Fixes and Improvements:
* Removed a bunch of crashes and memory leaks
* Improved performance when scrolling and resizing in a variety of ways
* Restored ability to launch on M1 Macs
* Decreased app size

## 2.0

Large scale changes to the entire app:

User Interface Overhaul:
* Modernized and native-ized user interface
* Toggle a sidebar in different modes next to or over the document depending on context
* Sidebar can be toggled using navigation bar buttons, keyboard shortcuts, and sideswipes
* Navigation bar and sidebar will use light or dark theme depending on the syntax theme being light or dark
* Added custom tint color
* Added support for multiple windows

Search:
* Added search mode to sidebar
* Search for content in the hexadecimal, ASCII, or binary column
* Preview results with context and jump to and highlight them in the document
* Jump between results with arrow keys
* Search results are limited to the first 1000 hits to increase performance

Analysis:
* Added analysis mode to sidebar
* Get information about the selection or the entire document
* Decode to integers
* See byte frequencies
* See detected file signatures (magic numbers)

Significant Performance Improvements:
* Document load times and scrolling performance is drastically increased
* Fixed crashes during (too fast) scrolling
* Fixed crashes during pinch-to-zoom
* Fixed crashes during opening documents
* Fixed crashes when putting the app into background

Misc Additions and Changes:
* Unified column reorder and hiding menu
* Mono Green themes split into light and dark
* Mono Green themes and corresponding icon changed to use app tint (solarized) green
* Options now show keyboard shortcuts next to them on iPad
* About screen shows version number
* Added changelog to the app
* Added symbols for newline (\n, 0x0a) and tab (\t, 0x09) characters
* Moved easter egg
* Changed the way the outer background is colored
* Rounded corners in secondary selection
* Removed little endian option due to backend changes

Misc Fixes and Improvements:
* Better support of Dynamic Text (Accessibility font size)
* Text rendering should be slightly sharper
* Improved scroll position after rotating or resizing
* The document no longer appears scrolled after opening on some devices
* The document browser no longer appears to rotate when opening a document
* Open from share sheet works reliably
* Slightly tweaked about screen order and icons
* Rudimentary cursor support for theme and app icon buttons

# Release 1

## 1.0

* Initial release!
