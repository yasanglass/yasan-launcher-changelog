# YASAN Launcher DEV Changelog

## Unreleased

- Fix App Options bottom spacer color.
- Apps clickable area on Drawer (Grid), Dashboard Folders, Search & Home is now rounded.
- Back buttons clickable area on Drawer & Dashboard is now rounded.
- If the other version of YASAN Launcher is installed the version information is now visible on Changelog screen.
- Apps version name & code is now visible on the bottom of App Options.

## 21.12-DEV-325

- Added App Pin switch to App Options (only available to Premium users).
- New "New Folder" button on App Options which opens the new folder screen and adds the app automatically on start.
- App Pin as a feature cannot be toggled anymore (its always enabled if you are a premium user).
- Fix drawer apps not being updated when an app is added/removed to/from a folder from App Options.
- Fix App Pin list items always using Rubik font.
- Fix App Pin list items paddings.

## 21.12-DEV-324

- Added App Hide options to App Options (only available to Premium users).
- Added Folder options to App Options to easily add/remove apps to/from folders.
- Long clicking Dashboard shortcuts now opens App Options.
- App Hide as a feature cannot be toggled anymore (its always enabled if you are a premium user).
- Some adjustments on when folder & dashboard shortcut data is refreshed.

## 21.12-DEV-323

- Fixed warning UI being blank somehow (previously used on Color picker screen).
- Now if the launcher is not set as the default launcher a warning will be shown on the main options screen.
- Segment titles on Color picker screen no longer have the extra spacer.
- Removed Advanced options screen and the "Change default home app" button is now moved to the main options screen for easier access.
- Added the option to show YASAN Launcher logo & version name on the bottom of Dashboard (disabled by default).
- Update to Compose v1.0.5 (from v1.0.4).

## 21.12-DEV-322

- Update Coil to v1.4.0 from v1.3.2 (~~fixes cross-fade bug?~~).
- Changelog data is now fetched from <https://github.com/yasandev/yasan-launcher-changelog>.
- Fix global events not being triggered if the new event is the same as the previous event.
- Major improvements & optimizations on how home button clicks are handled (fixes many weird behaviors).
- Fix long clicking apps on Search launching the app information screen instead of opening the app options bottom sheet.
- Add click labels for Buttons Box (accessibility).
- Fix some image content descriptions (accessibility).
- Use cross-fade for loading YASAN & YASAN Launcher logos.

## 21.12-DEV-321

- "App Icons" slider title is now renamed to "App Count" on Apps Box Options screen (included in 21.11-320 stable release).
- Optimized how apps list on Drawer is updated (applies only to the list view).

## 21.11-DEV-319 (RC-2)

- Optimized how New/Edit folder screen handles different folder modification events which fixes the duplicate message & multiple navigation actions when the modification is successful bugs (this introduces a new global event queue system to the whole launcher system that might be buggy in some heavy use cases, it will only ship to 21.11 if there are no issues reported).
- New/Edit folder screen messages now show as Toasts and not SnackBars as they are less annoying and can be shown for shorter durations easily (Is going to be replaced with a custom snackbar style soon).
- Folder apps are no longer excluded from Drawer by default.

## 21.11-DEV-318 (RC-1)

- App icons cross-fade animation can now be toggled on and off from Look & Feel options screen.
- Changelog text size decreased to 14sp (from 16sp).

## 21.11-DEV-317

- New "Icon Style" option for Buttons box which lets the user choose from 5 different icon styles.
- App options dialog is now shown as a bottom sheet.
- Dashboard Greeting's weekday text now properly follows the devices default locale.
- Remove widget support for 21.11 release.
- Fix Layout segment title disappearing if icons are disabled on Drawer Options screen.
- Added App Icon size preview to Apps Box Options screen.
- Added App Icon size preview to Drawer Options screen.
- Added App Icon size preview to Search Options screen.
- Optimize how the selected font family is fetched on different screens.
- Improve the icon placeholder highlight color.
- Search Options are now divided into two segments for easier use.
- "Icons" segment title is now renamed to "App Icons" on Drawer Options screen.
- "App Icons" switch title is now renamed to "Enabled" on Drawer Options screen.
- "App Label" segment title is now renamed to "App Labels" on Drawer Options screen.
- "Icons" segment title is now renamed to "App Icons" on Apps Box Options screen.
- "Apps" slider title is now renamed to "App Count" on Apps Box Options screen.

## 21.11-DEV-316

- Compose 1.0.4.
- Kotlin 1.5.31.
- Major app icon loading optimizations which greatly reduces the initial loading time & uses less memory.
- App icons now show a placeholder while being loaded.
- App icons now always have a cross-fade effect when being loaded.
- Fix AppWidgetHost memory leak (hopefully).
- Fix Drawer icon size preview not matching the icon sizes on Drawer.
- Adjusted app icon paddings.

## 21.11-DEV-315

- The exact app version is now shown on the Changelog screen & the Changelog buttons description.
- Fix widget list text color being black on night/dark mode.
- Fix changelog text color being black on night/dark mode.
- Fix Billing Client memory leak.
- Removed broken widget preview images.

## 21.11-DEV-314

- Now you can read the app changelog for both release channels on the new Changelog screen (it currently shows the raw markdown file without formatting but it will be improved soon).
- Added an Uninstall button on App Details Dialog which is only shown if the app can be uninstalled (Currently looks a bit weird but the whole App Details Dialog UI is going to get changed anyways).
- Improved default Home colors.
- Fixed Pride options screen having an invalid name.
- Added lots of missing button descriptions.
- Removed AI IQ & AI Performance user properties.
- Build time text on the About screen is now properly formatted to be easily readable.
- Misc. code quality improvements.

## 21.11-DEV-313

- The unstable/developer channel is now renamed to DEV since NEXT can cause confusion.
- Widget picker list (still very wip).

## 21.11-NEXT-312

- Kotlin 1.5.30.
- Compose 1.0.3.
- Small bug fixes & performance improvements.
- Fix some invalid icon content descriptions.
- Initial developer level Widget support which also includes a new set of buttons on the bottom of Dashboard.

## 21.11-NEXT-311

- Segment titles now have extra vertical spacing on top to make everything more separated and cleaner.
- Segment titles parent text is now on shown on top of title.
- Fix Icon Size Preview on Apps Drawer Options not rounding the corners of the item below it.
- Update all legacy sliders to optimize performance.
- Update Compose Accompanist to 0.19.0 (mainly effects view pagers like Home & Intro).

## 21.10-NEXT-308 (RC-2)

- Fix premium status update system being too strict causing premium to be disabled temporarily for premium users.
- Some optimizations on option sliders.

## 21.10-NEXT-307 (RC-1)

- Changed Color Picker Button's style.
- Changed Home Alignment Picker's style.
- Decreased divider width size (1dp from 2dp).
- Some optimizations on Intro & About screens.
- Start & End strings are now replaced with "Left" & "Right" as LTR is only supported yet.

## 21.10-NEXT-306

- The option to exclude folder apps from being shown on Drawer (Enabled by default).
- Optimized how apps are loaded into Drawer.
- Fixed typo in the message shown when Live Information fails to load on About screen.
- Default Home app icon size set to 72 from 64.
- Apps Box options screen is now more organized & Row/Column option is improved.

## 21.10-NEXT-305

- Improved the title text for dark & light color picker screens.
- Improved palette generation configuration.

## 21.10-NEXT-304

- The option to pick individual custom colors for light & dark UI modes.

## 21.10-NEXT-303

- Fix crash when apps are being loaded from system & the device is shutting down in the same time.
- Compose 1.0.2.
- Compile SDK set to SDK 31.

## 21.10-NEXT-302

- Fix crash when loading AI performance data if you previously had a very old version of the launcher installed.
- Fix "Icon" & "Icons" strings not being capitalized.
- Fix Premium screen crash when Sku details list is null.

## 21.09-NEXT-288 (FINAL)

- Fix crash when no activity could be launched for setting screens.
- Simplify build time stamp on About Screen.

## 21.09-NEXT-287 (RC-1)

- Full intro functionality.
- Removed some DEV tools.
- Disabled all image loading cross-fade animations due to being bugged in Coil.
- Fix primary and secondary colors being flipped in day/night themes for some elements.
- AI IQ & AI Performance are now a user property in analytics.

## 21.09-NEXT-286

- Navigation animations reverted back to simple fade animations due to slide animations not looking right.
- Vertical swipes on Home are now a little bit more sensitive (minimum drag amount decreased to 65 from 75).
- Improved analytical data collection (Home, Dashboard & Drawer screens being opened are now recorded as events & premium product key is a user property).

## 21.09-NEXT-285

- Compose 1.0.1.
- Navigation animation is now a horizontal slide but if the target screen is Home it is a simple fade animation.
- All images are now loaded using Coil Compose & have crossfade effect when being loaded.
- Force max one lines for folder names on Dashboard (If the folder name is long, it is going to be ellipsed).
- Fix Home gestures button description.
- Add App Pin button description.
- Improve Home Box button description.

## 21.09-NEXT-284

- Fix folder state not being updated in the proper order on Folder creation/edit screen.
- Fix crash after deleting a folder.

## 21.09-NEXT-283

- New Intro screen support. It currently only lets you boost some of your apps' AI score on the first launch.
- Compose 1.0.0 (Stable).
- Fix the bug where the initial value of apps status in folders edit screen was incorrect.
- Fix how back stack was handled internally which caused crashes with the latest version of Compose Navigation.
- Remove fake loading delay when opening folder information screen.
- Disable RTL support (layouts no longer flip horizontally when the device language is RTL).
- Disable folder edit's click ripple effect (should be fixed soon).
- Folder edit icon replaced from "Edit" to "ChevronRight".
- Folder edit clickable area is now the whole row instead of the icon only on Dashboard.
- A simple cross-fade animation is automatically added to all navigation actions due to updated Compose libraries.
- [TEMP] Android MinSDK set to 24 (from 23) due to a Compose issue.

## 21.08-NEXT-282

- ~~Fix the bug where the initial value of apps status in folders edit screen was incorrect.~~
- Fix layout corners on Premium screen when premium is enabled.
- Fix About screen's live developer information not being able to show failures.
- Home swipe actions are 3 times less sensitive now.

## 21.08-NEXT-281

- App pin support (works like the legacy app pin feature, will be replaced with a much more sophisticated system in next releases).
- Improved Premium Dialog style.
- Fix border color buttons not being named properly.
- Fix color picker screen showing "?" for border colors.
- Fix color picker screen not having the correct default value for border colors.
- Fix crash on drawer (hopefully).
- Fix switches description text being limited to one line.
- Fix switches not having the proper amount of padding when the description is long.
- Remove Premium related event trackers (bugged, will be replaced later).
- Remove Home Drag option (now always on).
- Add descriptions to Search options Switches.
- EASTER EGG #1.

## 21.08-NEXT-280

- Border width & color support for Apps Box & Buttons box.
- Fix options having non existent children list.
- Remove Fast Scroll feature.
- Fix Layout segment title on Drawer options not being always visible.
- Segment titles can now show the segment's parent.
- New edit button on folders to easily edit them without having to open options screen.

## 21.08-NEXT-279

- Previews now round corners of the content below them when expanded.
- Updated to Compose 1.0.0-rc02
- Fix Premium screen always showing the active premium screen.
- Fix rounded corners on Premium screen when Premium is disabled.

## 21.08-NEXT-278

- Fix more crashes related to loading icons.
- NEXT is now published in the beta channel instead of internal. It is still possible that some rare updates go to internal only.

## 21.08-NEXT-277

- Migrated to non-legacy UI elements on Search options.
- Fix crash when trying to load an icon for an uninstalled app.
- Fix crash when loading first label characters when app list is empty.

## 21.08-NEXT-274

- New improved floating page style on all screens.
- New icon size preview on Drawer options.
- Premium features list no longer always visible on Premium screen.
- Fixed the main options screen not recycling properly.
- Moved Fast Scroll switch to List options.
- Fix New Folder screen's title being "New Folder Options".
- Added a larger spacer below Dashboard items.

## 21.08-NEXT-273

- Add App Hide to Premium features list on Premium screen.
- Premium features list is now always visible on Premium screen.
- Cleaned up Drawer options screen to make it clearer.
- Fix Home previews letting user open app options dialog on long click.
- Home previews now have rounded corners once expanded.
- Home previews expanded state is now saved on device and restored properly.

## 21.08-NEXT-272

- Fix crash when trying to find the main user's serial.

## 21.08-NEXT-271

- Improved Work/Managed profile support.
- Improved icon loading system.
- Now whenever the launcher is restarted, it will go back to Home automatically.

## 21.08-NEXT-269

- New app loading system which supports Work/Managed Profiles.
- Work/Managed apps are now shown on Dashboard as a folder and not visible anywhere else.

## 21.08-NEXT-268

- Fix Home previews' background not showing wallpaper.
- Remove Bottom Branding from Dashboard.
- Remove Dark mode options from Look & Feel options screen.
- Convert Font options into a radio group instead of the legacy drop down menu.
- Remove unneeded divider on Search screen.
- Radio groups can now sort their items alphabetically if needed.
- New Gender queer, Gender fluid, Pan-sexual, Agender, Non-binary, Aromantic & Lesbian Pride flags.
- Renamed "LGBT" flag to "Rainbow Pride".

## 21.08-NEXT-267

- Fixed "No Results" text on Search not use the selected font.
- Improved Search screen style that does not cover all of the screen & has proper animations.
- If an app is launched from Search, Search screen will be closed automatically in the background.
- Fixed Color picker having x2 margin size.

## 21.08-NEXT-266

- New floating page style on all screens except Home.
- Fixed YASAN logo not being shown properly (by using Coil).
- Default home margin size set to 1.5 (down from 4.5).

## 21.08-NEXT-265

- "Loading Apps" indictors color is now automatically selected based on apps box background color.
- Added the option to select the amount each corner of Apps box & Buttons box should be rounded.
- Removed wallpaper modes.
- Removed wallpaper options screen.
- Removed vertical scroll option.
- Color picker screen now handles missing storage permission properly & shows a text if needed.
- Color picker screen now shows a text if it is unable to create a color palette using the wallpaper.
- New "Reset to Default" button on Color picker screen. 
- Support custom folder app icon size.
- Expand notification on swipe down.
- Launch Search screen on swipe up.
- Some new configurations set on the Manifest.

## 21.08-NEXT-263

- Color picker now shows 6 recent used colors.
- Remove buttons box border.

## 21.08-NEXT-262

- New advanced color picker screen.
- Custom color support for Frame background, Frame margin background, Apps box background, Buttons box background & buttons tint.
- Improved event tracking for Premium related events.
- Some small UI changes to make some options clearer.

## 21.08-NEXT-261

- Fix the ripple effect style on Shop & website icons on About screen.
- Simplified how the version name is shown on the Bottom Branding banner. It also now shows a build version and time of the build only on the About screen.
- Switches can now show a description below the title.
- New Pride options for Dashboard which currently lets you show a Pride flag on Dashboard (Currently supports LGBT, Bisexual, Asexual & Trans)
- New System Settings button on the options screen.
- New Advanced options screen which only lets you easily change the default home for now.
- Fix Search options screen title being "Search".
- New "Folders" segment title on Folder options screen.

## 21.08-NEXT-260

- New Shortcut settings option on Dashboard options. It currently lets you choose how your shortcuts are sorted.
- Dashboard clock is now always shown if Greeting is disabled.
- Dashboard clock text color is now the primary color (YASAN Blue) when the time is 11:11.
- Dashboard clock is now visible below the greeting text when a Greeting text is active.
- Fix the "crash" when the system is being shut down (dead) and apps are being loaded in the same time.
- Fix Dialog width size bug on Compose 1.0.0-rc1.
- Fix Premium information on Premium header on the main options screen not use the selected font.
- Fix Drawer item's sorting change with a delay when Drawer was opened.
- New Premium-Only Feature banner added. Currently only used on App Hide screen.

## 21.08-NEXT-259

- Improve Dashboard spacer sizes.
- ~~Added a progress bar when the shortcuts are loading.~~
- Compose version 1.0.0-rc01 ~~(should fix the keyboard issue on Search)~~.

## 21.07-NEXT-258

- Close app options pop up when the app information screen is launched.
- Fix ripple effect style for sliders.
- App options dialog now shows the app icon.
- Versions no longer have a special version name.
- Drawer App icons in grid mode now have more space around them on tablet devices.
- Remove Fast Scroll support from Grid Drawer.
- Option button's description is now a single line.
- App Hide is now locked for non-premium users (The premium dialog is a placeholder).
- The spacer between Dashboard items is now smaller.