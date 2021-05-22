# Release 2.1

## 2.1.9
* Fixed layout issues in sidebar on notched phones

## 2.1.8
* Highlight line and byte better with jump to offset
* Reduced alternating rows contrast in light rows
* Rounded alternating rows
* Updated to new website and mail and added new Twitter account
* Removed “jump to offset” from planned features
* Added context menus to social buttons
* Changed icon of the jump to offset button
* Changed the way the jump to offset field is implemented
* Added 2.1 Changelog

## 2.1.7
* Added button to jump to offset
* Added regex and case sensitivity filter options to search
* Added button to share search results
* Added context menu to search results
* Added option to select search result
* Removed slideover mode for sidebar so no content is ever covered
* Fixed search results not having the correct background color
* Fixed search results not switching theme correctly
* Added suggest theme button
* Fixed a crash when arrow keying up or down in search sidebar without results
* Probably fixed a crash that was caused by undefined layout for example at 0 font size

## 2.1.6
* Completely rebuilt document drawing from table to procedurally loaded single view paving the way for future progress and completely undid it all again because it caused too many issues
* Restored ability to select text when scrolling very far down
* Slight (invisible) improvements to drawing a selection
* Mentioned Bruno Philipe in about screen

## 2.1.5
* Updated App Icons
* Added “Shades of Purple” themes
* Added alternating rows option
* Added absolute count option to byte frequencies
* Fixed an issue where layout would be broken by some actions like changing font size through buttons or shortcuts 
* Fixed an issue where sometimes in the byte frequencies grid numbers like 0.995 would be displayed as .00 due to the byte being cut off
* Added HexFiend code page
* Added an option to reset all settings
* Enabled “Follow Dark Mode” by default
* Fixed space not being blue in EBCDIC
* Changed icon for text bytes in analysis sidebar
* Changed weights of some icons in about screen
* Updated launch screen
* Added new app icon to the easter egg screen

## 2.1.4
* Changed selected sidebar color style to be more similar to iWork apps
* Changed the way codepages are handled internally and removed caching. Combined with more deliberate UserDefaults reading this shound again massively increase performance
* Added code page and byte highlight selection buttons
* Code page name is now correctly represented in a bunch of places in the UI (not always ASCII)
* Added explanation for symbols and colors to format panel
* Improved the way drawing is handled again increasing performance
* Changed the way theme selection buttons are implemented to generalize them for code page selection
* Fixed selection not working in areas not visible before scrolling
* Fixed iPad cursor not working over center of byte
* Removed deprecated dependency probably further reducing app size
* Fixed byte frequency grid colors sometimes being too bright in dark mode
* Fixed a crash where an interaction between search and visible columns could lead to a crash (thanks @j0rn0r)
* Changed icon for Twitter feedback in analysis sidebar

## 2.1.3
* Added AppStore and app share buttons to about screen
* Restored ability to launch on M1 Macs
* Slightly increased line number contrast for accessibility
* Changed the contrast between the background and the secondary background
* Changed the way layout is handled internally which should result in smoother size changing (in preparation for an eventual macCatalyst version). Please report any issues you might find.
* Reduced frequency when hex grid is redrawn when changing size
* Fixed an issue where internal size computations erroneously assumed sidebar was visible
* Fixed another situation where changing a selection could result in it the selection being wrong

## 2.1.2
* Made search keyboard dismiss on scroll
* Made sidebar wider on notched phones in landscape
* Fixed search layout issue in landscape on notched phones
* About halved app size by improving the easter egg
* Fixed “Abbreviation Explanation” popup covering entire screen on iPhone
* Fixed another memory leak

## 2.1.1
* Added metadata section to the top of analysis tab
* Better accuracy when selecting text
* Fixed cursor snapping in ASCII column being wrong
* Fixed cursor snapping not working before first byte and after last byte of each line
* Sped up performance for some things like selection and some animations by caching frequently used value
* Increased selection performance by not running analysis in background when changing selection

## 2.1.0
* Indicate currently open sidebar
* Resolved some memory leaks after closing documents which could cause the app to crash after opening multiple documents
* Added iPadOS Cursor support when selecting or hovering over text
* Fixed an issue where altering a selection would sometimes cause it to reset
* Added indices and explanation to analysis byte frequencies grid
* Tweaked colors in analysis byte frequencies grid for better legibility
* Added cursor interaction to analysis byte frequencies grid
* Added secondary click (right click) support to interactable lables
* Added @c10um0 to acknowledgments section of about screen
* Sorted Twitter links in acknowledgments alphabetically—no favoritism!
* Fixed changelog in sidebar containing next headline

# Release 2.0

## 2.0.9
* Included 2.0 release changelog in app
* Fixed file size in analysis sidebar being off by exactly one byte
* Fixed byte frequency grid colors being wrong after switching between light and dark mode
* Fixed Analysis screen showing decimal places (zeros) for bytes

## 2.0.8
* Added selection analysis panel
    * Get information about the selection or the entire document
    * Decode to integers
    * See byte frequencies
    * See detected file signatures (magic numbers)
    * Functionality will be further expanded in the future
    * Please suggest anything else you’d like to see in this panel!!
* Added symbols for newline (\n, 0x0a) and tab (\t, 0x09) characters 
* Fixed open from share sheet not working when app has not been opened recently
* Fixed thin line artifacts in selection
* Made it easier to get to the easter egg

## 2.0.7
* Expanded sideswipe gesture to any amount of fingers and trackpad
* Build custom Markdown renderer for changelog
* Fixed issue where document would scroll a bit when opened
* Fixed issue where document browser would rotate when opening a file
* Tweaked search result highlight animation
* Reduced probability of title bar title and buttons being truncated
* Slight tweaks to the easter egg

## 2.0.6
* Added keyboard navigation to search
* Added animation to indicate search result
* Added sideways swipe to show or hide sidebar
* Slightly changed conditions for sidebar modes
* Removed little space at bottom of changelog page
* Slightly changed formatting of version number in about screen
* Did some work for future macCatalyst version:
    * Allow OS tint color override
    * Custom preferences window on Mac

## 2.0.5
* Increased scroll and search performance by increasing computing thread priority
* Limited search result count to 1000 drastically increasing performance while searching
* Fixed: Keyboard showing up when first opening app
* Fixed: Open from share sheet works again
* Fixed: Multiple issues where the app could crash in the background if something was ever selected
* Included changelog in app
* Updated planned features in about screen to no longer include no-longer-planned-because-already-implemented features
* Changed the order of some links in about screen
* Changed some texts in in about screen
* Changed the icons in about screen from bitmap to SF Symbols on a rounded rectangle and bitmaps on a rounded rectangle
* Changed some icons in about screen using SF Symbols

## 2.0.4
* Improved sidebar showing and hiding on iPhones and narrow iPad layout (some changes are iOS 14 only)
* Made search result actually show up on iPhones and in narrow iPad layout
* Improved search result preview layout
* Changed the way too long labels in info screen are handled
* Changed sidebar colors to be more sidebary
* Fixed position of search bar on notched iPhones

## 2.0.3
* Added search!
* Changed the way the outer background is colored. Opinions?
* Added Mono Green Light theme
* Caught some edge-cases during which pinch-to-zoom and sometimes opening a file would cause a crash
* Rounded corners in secondary selection
* Fixed toggle column shortcuts not working
* Draw font size label before showing the sidebar so it doesn’t suddenly pop up anymore
* Removed legacy code relating to old UI
* Changed version numbering scheme, removing unused 0

## 2.0.0.2
* Fixed: Sidebar and content scrolling horizontally in iPhone on landscape
* Fixed: Some labels being truncated in about screen by slightly increasing sidebar width
* Fixed: Theme buttons having weird spacing when toggling compact mode
* Fixed: A crash that sometimes happened where NaN bytes per line would be computed

## 2.0.0.1
* Changed UI to a regular navigation bar with settings on the right (pages style)
* Added custom tint color
* Changed Mono Green theme to use tint color (opinions?)
* Added version number to about screen
* Better support of Dynamic Text (Accessibility font size)
* Moved easter egg
* Fixed a lot of issues with changing settings in one window not transferring to another window

## 2.0.0.0
* Added support for multiple windows
* Significant performance improvements computing and precomputing colors and representations, this should result in faster scrolling and rendering
* Added keyboard shortcut display to settings on iPad
* Sharper text rendering (probably)
* Reworked the way settings work behind the scenes, this might cause crashes, please report all of those!
* The “Little Endian” toggle has been removed temporarily (is anyone using that?)

# Release 1.0

## 1.0.0.12
* Internal config tweak for App Review
* Changed en-dash at the very bottom of about screen to em-dash

## 1.0.0.11
* Fixed an issue, where the file browser would sometimes launch into light mode, even though there is a dark theme detected
* Adjusted some margins in about screen, to make link labels more readable and not just slightly truncate theme previews

## 1.0.0.10
* Actually fixed the issue with themes being broken when relaunching application from background with ‘follow dark mode’ enabled. Huge thanks to @mancifbier
* Added missing keyboard shortcuts for options “Binary Columns”, “Overscroll”, “ISO Latin 1 Codepage”
* Background accommodations for fastlane automatization

## 1.0.0.9
* Caved to popular demand and added an option to turn off “Binary columns”. With that disabled columns can now have any (whole) number of bytes and not just powers of two (1, 2, 4, 8, 16, 32, 64, 128, 256)
* Added an option to use the ISO Latin 1 codepage for more characters in the orange/yellow set
* Added overscroll option
* Added haptic feedback when closing document
* Added back in missing keyboard shortcuts
* In Acknowledgements section actually named “Textor” correctly. Thank you Appstore connect for keeping this feedback from me
* Very slightly tweaked they grey color in the Tomorrow Night theme
* Changed the order of themes in settings to not be chronological in order of addition
* Rotating the device now looks smoother
* Behind the scenes tweaks to automate screenshots

## 1.0.0.8
* Hopefully fixed sometimes light/dark mode becoming confused with “follow dark mode” enabled, when opening the app
* Made app icons look less pixelated through the magic power of antialiasing
* Added simplified roadmap
* Added link to the hot new website
* Fixed: Highlighting sometimes render as red
* Fixed: It crashed when speaking selection (Settings>Accessibility>Spoken Content>Speak Selection)
* Tweaked: Theme previews will be double with if compact and the screen is wide enough
These last two were reported by @Filippoclaudi

## 1.0.0.7
* Added ability to select text:
    * Double tap to select “word” between null bytes
    * Long press or tap-drag to select range
    * Copy or share text
    * Option to include spaces in share
    * Option to copy ASCII placeholder or true ASCII
    * !! There might be some bugs here. Please let me know if you encounter any issue, like crashes, inability to select text, the edit menu not being there or anything else
* Logically separated document viewer from menu. This might fix some minor issues. There might also be bugs, like weird overlap or options not working, please tell me! This *might* fix the overlap on the iPhone XR
* Added keyboard shortcuts for most settings
* Changed font to SF Mono since it is legal now (iOS 13)
* Hid an Easter Egg
* Added Context Menu to info button (iOS 13)
* Added an option to show the status bar
* Tweaked Haptics do be less aggressive
* Added debug information to feedback mail
* Tweaked some contrast on the light themes
* Added in app TestFlight link
* Removed iCloud Drive folder
* Added reference to hexyl – one of the original inspirations
* Toggling hexadecimal capitalization immediately displays in theme previews again
* Fixed Documents not correctly opening when using share or opening from the long press menu on the home screen when there was already an open document
* Fixed an issue where in some rare cases part of the line numbers would extend under the edge of the screen
* Options UI now generated procedurally. This makes it faster to add new ones in the future
* Updated to Swift 5, supposedly reducing app size

## 1.0.0.6
* Huge performance improvements for scrolling in large files
* Fixed an issue where caches would not be cleared correctly causing crashes with large files (@Filippoclaudi)
* Line numbers follow capitalization preferences
* Put the preferences in an order that makes more sense – or any really
* Icons now all have the same scale and weight
* Added pinch to zoom to change font size
* Slightly increased font size in font size label
* Added button shake when trying to set font size to impossible value or turn off last panel
* Added haptics support (let me know if you like or dislike it)
* Toggle things off that were already there
    * Line numbers
    * Turn off highlighting in any theme

## 1.0.0.5
* Minor scroll performance and loading improvements by computing colors in advance
* Automatically switch themes to follow system dark mode (iOS 13)
* Theme previews now always display all sample bytes. no more, no less
* The scrollbar on the right does not jump around after scrolling 1/3 of the way
* The GitHub icon is better recognizable in dark mode
* Scrolling with arrow keys now supported. This makes the entire UI navigable by keyboard (except for settings)
* Scroll to top by tapping the top of the screen
* New preferences:
    * Capitalize hexadecimal (FF or ff)
    * Compact mode (no spaces between bytes)
    * Little-endianness (requested by @Filippoclaudi)
    * Toggle theme switching
    * Half font sizes (like 14.5)

## 1.0.0.4
* Added rainbow icons
* Removed ability to create files. Editing is not yet supported anyways
* Shows file extension in iOS 13 (in principle, SDK is broken)
* Tweaked UI
    * It is symmetrical (iOS 13), due to squaring the close button (SF Symbols)
    * Has bigger icons for font size selector (iOS 13) (SF Symbols)
    * Following dark mode (top bar and about screen)
    * The UI bar should always have great contrast now (iOS 13)
* When launching in narrow SplitView on iPad the UI is displayed correctly immediately and not just after a fraction of a second
* Added context menus to font size and panel controls (iOS 13)

## 1.0.0.3
* Added visual theme switching
* Changed font size selection to buttons with current size indicator
* Added keyboard shortcuts for
    * Changing font size
    * Dismissing the document
    * Showing settings
    * Toggling columns
* Made launch screen obey dark mode
* Tweaked appearance of column order slider
* Increased font size upper limit to 35
* App no longer crashes when a single byte is too wide for the screen

## 1.0.0.2
* Fixed an issue where app would crash when opening empty files

## 1.0.0.1
* Fixed content overlapping with home indicator on home button less devices (thanks @j0rn0r)
* Fixed the notch on iPhone X style devices overlapping content
* Fixed font or theme selector not shown entirely (thanks @j0rn0r)
* Removed old code making the app smaller and a bit faster (in principle)
* Added line numbers
* Added binary column
* Added options to hide and reorder columns
* Added rudimentary dark mode support

## 1.0.0.0
* Open any file from within the app or through the share sheet
* View Hexadecimal and text representation for the file
* Load arbitrarily sized files instantly
* Byte highlighting (for ascii, whitespace, null byte, control characters, ...)
* Different color schemes and font sizes
* Switchable app icon
