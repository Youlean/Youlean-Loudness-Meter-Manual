# Changelog

**V2.5.11 - July 15, 2025**

*	Fixed crash when loading deleted default preset
*	Fixed crash when resizing GUI on Windows with OpenGL rendering
*	Fixed A/B state not working when graph saving is set to AUTO
*	Fixed Pro Tools crash when using bigger audio buffer sizes
*	Fixed reserve RAM buffers knob not working correctly
*	Fixed some app audio settings don't work correctly
*	Fixed crash when changing audio settings in standalone app
*	Fixed AAE -30002 error in Pro Tools
*	Fixed measurements start from silence after playhead jumps in Time Code mode
*	Fixed project files can not be saved on macOS
*	Fixed custom path for export doesn't work on macOS
*	Added option to automatically export measurements after AudioSuite analysis
*	Added normalization function when using "Render" button in AudioSuite
*	Added fonts for Japanese, Korean, Arabic, Thai, and Chinese languages
*	Added momentary and short term bar options
*	Added option to disable renaming of the normalized file
*	Added option to sync play head position when the playback is paused with Time Code histogram mode
*	Measurements won't reset when transport loops and Elapsed or System Time histogram mode is used
*	Max analysis time is now 24 hours (it is actually infinite, but you can preallocate RAM for max 24 hours to avoid audio dropouts)
*	Text scaling now scales max true peak values above the peak meters
*	Various small fixes

**V2.5.10 – November 9, 2024**

* Fixed graph memory not saving correctly
* Fixed utf8 characters not showing correctly in file names on Windows
* Fixed meter hidden when external monitor is disconnected
* Fixed file browse multimono crash
* Fixed clipped text when moving with hardware acceleration off
* Fixed crash when changing default OS audio device with standalone app
* Fixed broken chars in Windows App settings
* Fixed app will reset its settings if you quit via app menu a couple of times in a row
* Fixed AAE: -20038 error in Pro Tools
* App will now remember its position on the screen
* Added resizing from all sides of the window for App on Windows
* Removed meter interface is larger than the monitor warning
* macOS 10.13 is now minimum requirement
* Various small fixes

**V2.5.9 – October 3, 2024**

* Fixed default settings do not load correctly with VST3 in some DAWs
* Saving app session and dark theme settings are now global
* Updated handling AAX IDs for a possible final fix for -20038 error in Pro Tools
* Various small fixes

**V2.5.8 – September 26, 2024**

* Fixed crash when changing audio inputs in standalone APP
* Fixed not being able to change audio device in the standalone APP on macOS 14.1 or earlier
* Fixed normalized file name unicode error on Windows
* Fixed GPU acceleration can not be disabled in some cases
* Fixed overdubbing with Time Code mode not showing the right part of the graph
* Added a popup button to update all presets when you change some parameters
* The app will automatically reset audio input settings if it detects that it has crashed repeatedly
* Various small fixes

**V2.5.7 – September 13, 2024**

* Fixed uppercase letters in the file extension not recognized correctly when analyzing a file
* Fixed normalization not working for FLAC files
* Fixed normalization not working correctly for files bigger than 4GB
* Fixed graph glitches when framerate drops while overwriting in the time code mode
* Fixed macOS scaling using CTLR instead of COMMAND key
* Fixed crash in Qlab 5 on macOS
* Fixed app won’t scale correctly on Windows when moving between monitors with different DPI
* Fixed the “GUI will not fit” warning wrongly showing when using vertical monitors
* Fixed AAX plugin doesn’t load in Avid Media Composer
* Fixed AAX AAE: -20038 error in Pro Tools
* Fixed graphical glitch when graphs are updating
* Fixed compatibility with older project files
* Added “–unregister-license” option to unregister license from the command line tool
* Added more graph window sizes between 1h and 4h
* Added option to double click and edit window size. Use: 01:15:53, or 1h 15m 53s notation. If time is not specified, it will be treated as minutes
* Added option to auto update graph window size from the input audio length
* Added default audio device option for input and output in the standalone app
* Added option to reverse mouse wheel zooming direction
* Added peak meter scale options
* Added option to analyze system audio natively on macOS 14.2 and later
* Added license info panel in registration menu
* Added “Reset All Settings” button in the help menu
* Updated the handling of global settings
* Presets now save all settings, including text scaling etc.
* Graph saving option no longer requires PRO version
* Improved project saving speed and reduced project file size
* Improved Audio Unit stability
* Reversed direction of mouse wheel graph zooming
* Windows app when analyzing system audio will auto switch audio devices if the default device is changed
* Switched normalization WAV format for files bigger than 4GB from W64 to RF64 for better compatibility
* Increased maximum file analysis time to 5965 hours (tested up to 150 hours)
* Input file is not required anymore to register the license in the command line tool
* App will now always start centered on the screen in order to prevent it from being off-screen in multi monitor setups
* Various small fixes and stability improvements

**V2.5.6 – December 29, 2023**

* Fixed broken GUI text in drag & drop when GPU acceleration is off
* Fixed GUI lag when overwriting measurements in Pro Tools
* Fixed crash in auval tool on macOS
* Fixed crash with VST3 in Reaper on macOS
* Fixed audio output broken in Audacity with VST3
* Fixed top and bottom bars not hiding after project reload
* Updated CSV export file to include all measurements
* It is no longer mandatory to use “–export” for exporting in the command line tool
* You can now use “–preset-import-path” to import a preset from a custom location via the command line
* Various small fixes and stability improvements

**V2.5.5 – November 22, 2023**

* Added 49 new channel configuration options
* Added a button to quickly copy current measurements summary in the clipboard
* Added a system to check if audio input is detected, and host playback is paused preventing measurements in
* Elapsed histogram mode
* Added ability to analyze up to 24 channel audio
* Added ability to register the PRO version from the command line tool
* Added option to always show all channels for peak meters
* Added option to force multi-mono export for normalized file
* Added option to hide full file paths in exports
* Added option to write BWF metadata to normalized files
* Drag and drop file info text will show file name only
* Fixed crash when GPU acceleration is disabled.
* Fixed message box showing the same messages concurrently
* Fixed resetting bug when rendering in SADiE
* GUI scaling was reset to a default value
* Holding CTRL + ALT on Windows, or Command + Option on macOS and dragging the resize corner will scale the meter interface
* Improved compatibility with SADiE
* Improved design for standalone app preferences
* Improved general stability
* Peak meters will now automatically resize based on the channel count.
* Plugins and standalone app will now automatically select the best audio channel preset for you (if the feature is available in the host)
* Updated GUI scaling code. Windows will now support per-monitor DPI scaling
* Using multi-mono files for normalization will now export multi-mono files instead of the single file
* You can now analyze and normalize 1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16, and 24 channel audio.

**V2.5.4 – July 19, 2023**

* Fixed text summary and Command Line true peak max showing max short term value
* Fixed “USE DRAG & DROP FILE NAME” not working for file export
* Fixed crash when trying to change the export name on some Windows 10 systems
* Fixed GUI glitches with the free version
* Disabled double click to reset scaling on the resize corner
* Added license version info to the help menu

**V2.5.3 – July 10, 2023**

* Added 3s and 5s windows sizes
* Added 8k and 16k image export resolutions
* Added a helper panel for showing drag and drop channel configuration
* Added ylm2 command line tool that can be used for analysis, normalization, and file export
* Added ability to analyze FCPX clips directly with drag and drop
* Added auto width expand export option
* Added Dolby Media Meter CSV export
* Added export range options with BWF metadata support
* Added file browse panel for selecting individual and multi-mono files
* Added more content options like drawing a true peak graph
* Added option to automatically export graphs after analysis
* Added option to bold loudness target line in the graph
* Added option to bold true peak max line in the graph
* Added option to disable drag and drop normalization
* Added option to disable finish animation after drag and drop
* Added option to disable or enable graph fill
* Added option to hide top and bottom bars on the interface
* Added option to import/export presets
* Added option to select a more dense scale, or streaming scale where -14 is always visible
* Added option to select graph sampling type. This will affect the graph’s appearance when you use a long zoom size.
* Added option to select monochrome, horizontal, or vertical graph coloring
* Added option to select the normalization file format
* Added option to show all measurements export option
* Added option to show color thresholds as a background below the graph
* Added option to show color thresholds numbering on scale
* Added option to use drag and drop folder path for export
* Added path stroke export options
* Added Recalculate Selection Technology. Select the part of the graph you want to recalculate
* Added system default option for app audio sample rate
* Added test files that can be used for analysis and normalization in free and PRO version
* Added text summary file export option
* Added true peak graph histogram view
* Apostrophes are now allowed in the export file name
* Auto reset will automatically be disabled if using time code mode
* File export will now exclude the start offset
* Fixed audio glitches when using low buffer size and high sample rate
* Fixed crash when switching the A/B states
* Fixed crash when trying to replace the exported file
* Fixed dialogue percentage not saved in graph export
* Fixed double click to enter a value not working for alerts when the relative scale is active
* Fixed drop-down menu not responding on macOS
* Fixed hang on load
* Fixed Pro Tools AudioSuite in some cases cuts measurements if previous measurements are not cleared manually
* Fixed Pro Tools crash when saving a session
* Fixed the “audio processing deadline was not met” problem when working at 10h timeline
* Fixed true peak alerts showing in the histogram graph if the true peak threshold is hit
* Fixed Windows crash with mp4 drag and drop
* Fixed Windows installer always adds a desktop icon
* GUI drawing is 2x faster. When working in time code mode, speed up is even more significant
* Histogram position will not change if the playback is stopped and time code histogram mode is used
* Image export timeline will switch to time code if using time code histogram mode
* Improved start-up speed
* Input gain correction is now app setting only
* Lowered brightness of “Created with Youlean Loudness Meter” on export pictures
* Normalization now supports input files greater than 4 hours in length
* Optimized drag and drop and increased speed by up to 3.7x times
* Plugin loading is now 34% faster
* Project saving is now 10x faster.
* Removed 32-bit AAX plugin support for Windows
* Removed graph reset when switching the histogram mode
* The audio driver is now disabled by default for standalone APP
* The dynamics color “knob” improved the handling of the mouse clicks
* The dynamics color button will now be displayed with the gradients like in the graph
* The meter will now smartly exclude all data at the start of the time code if necessary
* Updated targets UX
* You can now click on the “PAUSED” text to resume measurements
* Added ATSC A/85 DIAL preset

**V2.4.4 – April 1, 2023**

* Added support for AAX Apple Silicon native

**V2.5.2 – BETA – April 25, 2022**

* Fixed crash when showing a message box

**V2.5.1 – BETA – April 24, 2022**

* Fixed normalization bug
* Fixed window resizing bug

**V2.5.0 – BETA – April 23, 2022**

* Fixed APP crash when unplugging audio device on Windows
* Fixed AudioSuite not resetting before analysis
* Fixed PDF export missing some peaks in the true peak graph
* Fixed a nasty bug causing crashes when having multiple plugins loaded at the same time. (might improve stability overall)
* Fixed app freeze when changing audio driver type on Windows
* Fixed app not closing completely in some cases on Windows
* Fixed crashes for Windows standalone app and bad audio drivers
* Fixed message box blocking UI on macOS
* Fixed some alerts shouldn’t change when relative loudness scaling is activated
* Added AES Streaming Short Form preset (commercials <60s)
* Added ITU-R BS.1770-1 DIAL and ITU-R BS.1770-2 DIAL presets
* Added an ability to test drag and drop in the free version with test files
* Added audio pass through option for the standalone app
* Added file loudness normalization with WAV export
* Added min alerts for momentary, short term and true peak hold readouts
* Added normalization verification for double checking normalized file
* Added option to require target hit for normalization
* Added preset popup infobox
* Changed view settings icon
* Disabled multi-mono plugin type in Pro Tools
* Enabled all histogram modes in standalone app and plugin hosts that don’t support these features. Auto reset will not function in some cases.
* Improved preset system
* The minimum OS version for macOS is now 10.11
* Old custom presets will auto upgrade to the new presets
* Reduced vertical size of the interface
* Removed 32-bit AAX plugin on Windows
* Under the hood optimizations
* Updated AAX SDK to the latest version
* Updated VST3 SDK to the latest version
* Other small UI, UX improvements

**V2.4.3 – February 14, 2021**

* Fixed choppy scrolling in menus on macOS
* Fixed forced dedicated GPU switch on macOS. Now the current GPU will be used if possible
* Fixed default preset not loading correctly
* Fixed loading custom preset does not change the GUI size
* Fixed meter in FCPX getting disabled in Big Sur
* Fixed OS preventing editing files after drag and drop
* Fixed using multi-file drag and drop could lead to incorrect analysis if channel settings are preselected
* Fixed app moving up when resizing the window on macOS
* Fixed installer not working in 32 bit Windows
* Fixed potential huge RAM usage with VST3 plugin
* Fixed GUI flickering in some DAWs on older macOS systems
* Fixed Time Code not working in some situations in Pro Tools
* Updated VST3 SDK to the 3.7.1
* Added support for Apple Silicon
* Added warning when sample rate is incorrect in the app
* If the sample rate is missing in the app preferences, a default sample rate will be used
* Removed momentary window knob
* Simplified buffer settings in the app preferences
* Ignore master volume setting in app preferences is now disabled by default
* Changed view settings icon (hopefully more clear now)
* macOS 10.9 is now a minimum system requirement for macOS
* Other small UI, UX improvements

**V2.4.2 – October 19, 2020**

* Fixed graph constantly resets in some DAWs
* Fixed file export not showing dialog values if dialog gating is selected
* Fixed app doesn’t remember the custom export path
* Fixed crash with macOS El Capitan
* Fixed crash with macOS Sierra
* Tested and ready for macOS Big Sur
* Improved preferences panel for standalone application

**V2.4.1 – October 4, 2020**

* Fixed VST plugin not showing inside EDIUS
* Fixed VST3 constantly resetting in Adobe Audition
* Fixed AU plugin not working on some older macOS versions
* Fixed crash that can occur if loading saved project and using timecode with the auto-reset off
* Fixed loudness target knob using frac position when manually setting
* Fixed CPU spike when resetting the graphs
* Fixed audio dropouts when using higher sample rates
* Fixed FCPX muting channels when rendering and using 5.1 channel configuration
* Fixed slow analysis with lower sample rates
* Fixed mono mpg files do not work with drag and drop on Windows
* Fixed drag and drop not working with mono or multichannel AIFF files on macOS
* Fixed true peak max value sometimes not shown in the excel export
* Fixed true peak not correct on mouseover when the relative scale is used
* Fixed export creating incomplete graphs for PDF and SVG files
* Fixed SmartScreen warning on Windows
* Fixed crash with VST2 and DAVID MultiTrack Editor
* Fixed crash in Cakewalk
* Fixed crash with VST2 and Wavelab
* Fixed crash with Adobe Audition
* Fixed crash with Adobe Premiere Pro
* Fixed crash with Soundforge Pro 12
* Fixed crash when analyzing huge files on Windows
* Fixed audio glitches when using VST2 inside Adobe Premiere Pro
* Fixed big ram usage when analyzing big files
* Improved VST2 stability in some daws
* Improved VST3 stability in some daws
* Rewritten GUI engine. Hardware acceleration is now supported
* If hardware acceleration is not supported, software rendering will be used
* Added hold CTRL to set the default preset in the drop-down menu
* Added option to show both integrated relative and dialog gated readout at the same time
* Added Analyze File menu item on the standalone application
* Added HBO, Disney+, EBU R128 S2, and EBU R128 S2 Music streaming presets
* Added remaining time info for drag and drop
* Added support for RF64 WAV encoding for analyzing 4gb+ files
* Removed message box information when exporting graphs
* Removed support for macOS 10.7
* Analyze multi mono files as one file by using .L.wav, .R.wav, etc. extensions with drag and drop
* Changing the preset won’t reset the measurements unless required
* Collapsed groups inside drop-down menus are now saved globally
* Changed color of the focus rectangle in order to make the text more readable
* The export custom path will be globally retained
* Other small UI, UX improvements

**V2.4.0 – March 20, 2020**

* Fixed macOS Mojave or Catalina can’t analyze audio from inputs
* Fixed crash with Vegas Pro when rendering
* Fixed crash with SADiE 6
* Fixed crash with OBS Studio
* Fixed drop down menus not scrolling in some cases
* Fixed reset button doesn’t clear all values in some hosts
* Fixed switching from A to B state doesn’t switch properly
* Fixed long non-ASCII filenames breaking GUI with file analysis
* Fixed standalone app not starting the audio engine after the first install on macOS
* Fixed standalone app crashes if digital inputs are selected
* Fixed plugin always starts in default size
* Fixed window resizing in Ozone 9
* Fixed dynamic range graph color do not update on preset change
* Fixed channel selection menu not showing correctly with histogram disabled
* Fixed short term alerts not set and reloaded properly in free version
* Fixed edited preset indication not working for streaming services
* Fixed tooltips showing wrong info if menus are open
* Fixed window resizing with OBS Studio
* Fixed crash when doing drag and drop on AudioSuite in Pro Tools
* Fixed drag and drop not switching to 5.1 channels automatically
* Added option to save and load projects with the standalone application
* Added option to export only loudness or dynamics graphs
* Added option to set points density for graph export
* Added option to the export-import graph memory file
* Added dialog gating option based on Dolby Dialog Intelligence
* Added option to see a voice detection inside the histogram based on Dolby Dialog Intelligence
* Added option to ignore system audio volume on Windows standalone app
* Added option to always keep the standalone app on top of other windows
* Added option to resize the window by its sides
* Added option to auto update export name based on the file name from drag and drop
* Added option to select integrated relative gate type
* Added option to select adaptive dialog gate method of calculation
* Added adaptive gate threshold setting
* Added configurable averaging window for the momentary loudness calculation
* Added integrated relative gate indication in the histogram
* Added option for showing an alternative look of the metering bars
* Added Netflix preset
* Added Deezer preset
* Updated YouTube preset
* Removed click to pause histogram tracking option
* Improved CPU usage when the UI is minimized
* Improved measurements naming in the graph export
* Changed indication for edited preset to a simple star symbol
* Output settings are removed on the standalone app because they are not needed
* The standalone app now remembers its position
* Integrated alerts are now set with presets automatically
* Successful export message box now shows the full path of the exported file
* Advanced optimizations are now on by default
* Improved project saving speed with large graphs
* Improved loading speed
* Changed LK indication to more correct LU indication
* The standalone app preferences will be reverted to default values
* Windows installer now remembers previous install paths
* Improved GUI performance on 5K iMacs and macOS running non-default display color profiles
* Other small UI, UX improvements

**V2.3.2 – October 17, 2019**

* Fixed wrong channel selection in the standalone app
* Fixed wrong input name with the ASIO driver in the standalone app
* Fixed GUI not working in some older macOS versions
* Fixed crash when changing GUI scaling and reverting back to original
* Fixed drop-down menu glitch
* Fixed drag and drop not working with Ogg files on Windows
* Removed support for 32bit on macOS
* Improved file support for drag and drop
* Added System Audio monitoring in Windows standalone app
* Added fullscreen mode in the standalone app
* Other small UI, UX improvements

**V2.3.1 – August 30, 2019**

* Fixed volume boost in FL Studio
* Fixed custom preset glitch
* Fixed blue window showing with empty buttons
* Fixed AAX plugin not loading with 7.1.2 channel configuration
* Fixed AAX plugin won’t load in Pro Tools 12.7 or earlier
* Improved compatibility with Pro Tools
* Added prevention of crashing when loading saved state from newer versions
* Audio is now only passed for channels set inside the interface

**V2.3.0 – August 11, 2019**

* Audio is now always passed for all connected channels
* Added option to add a custom logo to exported files
* Added a file selector button for quick analysis
* Added Amazon Alexa and Amazon Music preset
* Added tooltip info bar
* Added support for 7.1 surround and 7.1.2 Dolby Atmos
* Added true peak clipping channel indicator
* Added an option to invert time code for Elapsed and Continuous histogram mode
* Added AAX Audio Suite analyze button
* Added back support for 32 bit on macOS
* Time coding info is now inverted by default for Elapsed and Continuous histogram mode
* Time coding info is now always inverted after drag and drop
* Application will not start with paused measurements by default anymore
* Fixed macOS installer not showing all information if the dark theme is selected for the OS
* Fixed drag and drop has a wrong start in the Time Code mode
* Fixed drag and drop not working in some DAWs like Cubase
* Fixed GUI glitches with drag and drop in some DAWs
* Fixed spike at dynamics graph start
* Fixed crash when working with 5.1 surround channels
* Improved general stability
* Small UI, UX improvements

**V2.2.4 – June 20, 2019**

* Added Apple Podcast and Spotify Loud presets
* Drag and drop now always process audio at the file sample rate
* Measurements won’t be reset if you open a project with a different sample rate
* Alerts now show “OFF” when disabled
* Adjusted thresholds and rounding
* Adjusted Auto Gradient for dynamic range target to show all green when above the threshold
* Right click on readouts now opens the alerts settings
* Fixed graph jumps at 0 position when DAW is not playing when using Time Code mode
* Fixed some graphical glitches when working in Time Code mode
* Fixed mouseover dynamics graph showing dB instead of LU
* Fixed drop-down menu graphical glitch
* Fixed Pro Tools run out of power when using the Time Code mode
* Fixed Time Code not working on sessions longer than 14 hours
* Fixed slow GUI animations on some systems
* Improved the GUI performance, especially on macOS retina screens
* Improved overall performance
* Other small UI, UX improvements

**V2.2.3 – May 2, 2019**

* Fixed graph not correctly updated in some cases if using Time Code mode
* Fixed input gain not retaining value if global settings are used
* Fixed input gain does not modify the output anymore
* Fixed crash in TwistedWave with AU
* Fixed drag and drop info does not display correctly in TwistedWave
* Fixed wrong end position when doing drag and drop in Time Code mode
* Fixed crash with drag and drop on macOS Mojave if you have not allowed the permission to use audio
* Fixed graph not zooming correctly with mouse wheel if GUI scaling is not at 100%
* If you cancel drag and drop the graph is not reset anymore
* Animations are now a bit slower on macOS
* Removed halo around the dynamic graph

**V2.2.2 – macOS Only – April 25, 2019**

* Fixed problems with loading the plugin on macOS

**V2.2.1 – April 23, 2019**

* Fixed plugin reverting from PRO to free in some cases
* Fixed crash in Ableton Live 9 when loading more than one plugin instance
* Fixed drag and drop not working in Windows with non-English file paths
* Fixed drag and drop crashing with longer files
* Fixed crash when using 5.1 in the standalone app
* Fixed AAX not working on macOS
* Reduced RAM usage for drag and drop by 300%
* Improved speed of drag and drop by 2x
* Improved preferences panel in the standalone app
* Improved news panel
* Added option to check updates for BETA versions
* Added dropped file info on the histogram
* Added option to autosave app session
* Added option for input gain correction
* Drag and drop can now open all OS supported audio/video files
* Audio is now silenced while drag and drop analysis is performed
* The installer on macOS now recommends reboot or logging off, but does not force anything

**V2.2.0 – BETA – March 29, 2019**

* Added drag and drop to analyze WAV, MP3, OGG or FLAC files
* Added Excel file export option
* Added color alerts to mouse over readouts
* Added confirmation box when changing GUI scaling
* Added A/B save states
* Added DR guides in the histogram
* Added standalone 64bit app for Windows and macOS
* Removed support for 32bit on macOS systems
* Removed requirement for a reboot of macOS after updating the plugin using the installer
* Removed getting started screen
* All plugins and apps are now digitally signed
* Fixed wobbly graphs
* Fixed wrong selection position after session reload
* Fixed plugin starts in extremely low FPS mode after first use
* Added automatic gradient setting for dynamics graph
* Improved GUI performance
* Improved zooming on the histogram
* UI and UX improvements

**V2.1.1 – November 29, 2018**

* Fixed Sound Forge not starting in continuous mode
* Fixed opening an old project might give you low FPS
* Fixed typo in refresh rate menu
* Fixed graph not updating in timecode mode
* Fixed label text not scaling
* Fixed export not working on macOS
* Fixed Pro Tools reset graphs glitch
* Fixed SVG and PNG not exporting at correct DPI
* Plugin moved to Sound Field menu in Pro Tools

**V2.1.0 – November 23, 2018**

* Added plugin dark theme
* Added export white theme
* Added PNG, SVG graph export
* Added resolution selector for the export
* Added text scaling option
* Added option to save a custom presets
* Added simple way to unregister the plugin
* Added graph refresh rate control
* Added 1.5 HRS, 2.5 HRS, 3.5 HRS window sizes
* Added EBU S1 and ASWG presets
* Renamed PLR-Integrated to Peak-Loudness Ratio
* Renamed PLR-Short Term to Dynamic Range
* Extended range of true peak alert threshold (10dB to -30dB)
* Improved graph timeline text
* Improved loading speed
* Graphs rendering optimization
* Fixed crash in Studio One on macOS
* Fixed FL Studio wrong timecode position after project load
* Fixed plugin won’t work until you reselect the continuous mode in some DAWs
* UI and UX improvements
* Stability improvements

**V2.0.2 – September 23, 2018**

* Fixed graphical glitches on macOS retina screens
* Fixed plugin resetting to the FREE mode in Final Cut Pro X
* Fixed “GO TO WEBSITE” button
* Fixed update notification not working in Windows in V2.0.1
* Fixed plugin freeze if you pause measurements and disable and re-enable the plugin in the mixer
* Improved compatibility with vMix

**V2.0.1 – September 9, 2018**

* Fixed not being able to click on View and Registration menu
* Fixed plugin is moved to the bottom on retina screens
* Fixed resize error when dragging plugin from retina to non retina screen
* Improved compatibility with retina screens
* Improved compatibility with Final Cut Pro X (more work needs to be done)
* Fixed crash with AU loading in Studio One

**V2.0.0 – September 1, 2018**\\

* Fixed resizing issues in Ableton Live on Windows
* Fixed drop shadow glitch with scaled GUI
* Fixed problem with file names when exporting PDF files
* Fixed Elapsed behavior when “Auto Reset” feature is turned off
* Fixed plugin not working in FL Studio using AU plugin format
* Minor graphics fixes
* Added option to close “Window can not fit the screen” popup

**V1.9.9 – BETA – July 20, 2018**

* Improved GUI performance
* Added GUI animations
* Added preview for PLR histogram
* Fixed not being able to see the GUI interface
* Fixed not being able to resize GUI interface in vMix
* Fixed empty 2 button panel on GUI open
* Added registration panel

**V1.9.8 – BETA – June 28, 2018**

* Fixed “Pro Tools ran out of CPU power” bug
* Added Audio Suite version of the plugin for Pro Tools
* Changed GUI design (still work in progress)
* Added option to check for updates from the plugin
* Added “Pause Measurements” button
* Added option to set focus on readouts
* Resizing performance improvements

**V1.9.7 – BETA – May 7, 2018**

* Fixed hold max values not resetting after a mouse click
* Added AAX plugin type for macOS and Windows
* Stability improvements

**V1.9.6 – BETA – May 2, 2018**

* Fixed VST3 not working in Studio One
* Fixed VST3 not working in vMix
* Fixed bug when moving color splits will freeze vMix

**V1.9.5 – BETA – May 2, 2018**

* Added settings for PLR graph, alerts, optimizations
* Added pdf export option
* Fixed PLR-I measurement error after project reload
* Optimized binary size
* Reduced CPU usage by \~30%
* Minor GUI tweaks

**v1.9.4 – BETA – Apr 1, 2018**

* Fixed forced mono audio
* Fixed some crashes

**v1.9.3 – BETA – Apr 1, 2018**

* Fixed broken v1.9.2 build that will crash sometimes

**v1.9.2 – BETA – Mar 31, 2018**

* Added loudness target knob
* Added check if a plug-in interface can fit the monitor screen
* Added buttons to reset window size and scaling
* Added loudness range display
* Fixed crash when switching to 22050 Hz sample rate
* Minor GUI bug fixes

**v1.9.1 – BETA – Feb 28, 2018**

* Fixed Time Code behavior when “Auto Reset” feature is turned on
* Minor small bug fixes

**v1.9.0 – BETA – Feb 7, 2018**

* Added smooth color transition option
* Added PLR-Short Term and PLR-Integrated readouts
* Added second color split
* Added true peak graph display
* Added Getting Started window
* Added true peak graph display
* Extended range of true peak threshold to -30 dB
* Optimized graphics for macOS retina and Windows HiDPI mode
* Optimized graphics performance
* Fixed preset recalling
* Fixed most of the resizing problems on macOS
* Better compatibility with macOS High Sierra using AU format
* GUI design improvements
* Stability improvements

**v1.5.0 – BETA – Jun 4, 2017**

* Added GUI scaling. Activate by ctrl+drag on resizing handle
* Added view modes
* Added continuous mode
* Added fine control for true peak threshold
* Fixed crashes in Cubase – VST3 version
* A lot of stability improvements
* Minor graphical glitches fixes

**v1.0.5 – Jan 12, 2017**

* Added macOS installer
* Fixed settings not sticking after project reload
* Fixed jump when changing window size with the mouse wheel
* Improved scrolling with histogram control
* macOS stability improvements
* Minor graphical glitches fix

**v1.0.4 – Dec 12, 2016**

* Added manual.
* Fixed small bug when switching from auto to non-auto in Time Code mode
* Fixed wrong integrated and loudness range measurements if play position has jumped in the playlist

**v1.0.3 – Dec 8, 2016**

* Fixed random resetting transport in Bitwig Studio
* Many fixes regarding transport

**v1.0.2 – Dec 6, 2016**

* Fixed AU crash at load in Ableton Live
* Fixed true peak detection
* Fixed a button that pauses integrated and loudness range measurements

**v1.0.1 – Dec 4, 2016**

* Fixed missing libraries on macOS
* Fixed volume boost in FL Studio
* Fixed FL Studio crash while detaching the plugin
* Fixed Reaper crash after play in Windows
* Fixed minor graphical glitches

**v1.0.0 – Nov 30, 2016**

* Initial release
