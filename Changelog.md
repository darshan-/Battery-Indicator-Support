# BatteryBot Changelog

Describes changes in both Pro and Free versions of BatteryBot Battery
Indicator for each release since v3.0.0

## Contents

* [Pro Version](#pro-version)
* [Free Version](#free-version)

<a name="pro-version">
## Pro Version

v11.0.4

 * Made time diffs in logs more human friendly.
 * Added option to show seconds in timestamps in logs.
 * Not Charging no longer treated as Unknown in logs.
 * Changed how CSV file is exported to be compatible with Android 11. Allows user to select save location, removal of the WRITE_EXTERNAL_STORAGE permission.
 * Modified layout and sizing of elements on main screen: more flexible and better supports modern tall screens.
 * Updated build tools, support libraries.
 * Target/compile for API level 30.
 * Various clean up, reduction of APK file size.

v11.0.3

 * Disabled notification badge by default for main channel.
 * Updated build tools.
 * Updated target audience.

v11.0.2

 * Fixed problem with widget-only mode (no notification) on 8.0+ devices (XX%).
 * Added multiplier option to current hack.  (Can swap negative/positive, and on some devices can fix 0 mA.)
 * Some fixes and improvements to AlarmEditActivity around Notification Channels.

v11.0.1

 * Brought notification icon colors back, since some devices still support them on current versions of Android (Samsung seems to, at least).
 * Raised default priority for main Notification Channel (brings icon back to status bar by default) on Pre-9.0 versions of Android.
 * One Notification Channel per alarm type, for more granular control of alarm settings.
 * Initial Hindi and Farsi translations.

v11.0.0

 * Support for Android 8.0, 8.1, and 9.0 (Oreo and Pie), particularly Notification Channels.
 * Several bugfixes, mostly minor.
 * Efficiency improvements.
 * Initial Hebrew and Serbian translations.
 * New "Temperature drops below" alarm type requested by user as GitHub issue #4.

v10.0.4

 * I'm so sorry for the frequent releases this week, folks.  I'm fixing
   my bugfix again.  This is an issue that only affects a small
   minority of users, but it's important to get it right.  I really
   think I've got it this time.

v10.0.3

 * Fix (I think) rare crash introduced in last release.

v10.0.2

 * Performance and stability improvements.

v10.0.1

 * Bugfix: Remove timestamp from main notification
 * Bugfix: Vibrate alarms properly (please email me if any new issues arise)

v10.0.0

* Support Android 6.0+ (Marshmallow), including new permission model (ask as needed rather
   than at install time)
 * Support Android 7.0+ (Nougat), including split-screen view
 * Many significant improvements in performance, stability, and memory efficiency
 * Convert AlarmsActivity to a Fragment and place to right of Current Info
 * Notification Wizard: makes it easier to adjust how notification is shown
 * Option for another method to determine mA current
 * Updated Japanese and Chinese translations
 * Include boot event in logs
 * Add privacy policy
 * Use Fahrenheit by default for en-US and es-US locales
 * Check for notifications being blocked, warn user and link to settings to unblock
 * Remove finish_after_battery_use option which hasn't made sense in years
 * Many minor fixes

v9.0.1

* Fix bug where app wouldn't always close when Close selected from menu (e.g. after rotation).
* Fix bug where 1x1 circle widget showed up as 2x2 on some launchers.
* Make circle widget the same size as a launcher icon, even when the desktop grid gives
  it more space than that.
* Removed shadow from below battery graphic in main screen, which was not noticeable on most devices
  but looked ugly where it was noticeable.
* Added xxxhdpi launcher icon.
* Don't show redundant 'Fully Charged' in the prediction (time remaining) area of the main screen,
  but rather indicate with an mdash that there is currently no prediction.
* Updated traditional Chinese translations.

v9.0.0

* Redesigned main screen to look better, be easier to find the
  information you're looking for, and provide more information.

NOTE: As part of this redesign, the disable-lockscreen functionality
has been moved to a new app called <a
href="https://play.google.com/store/apps/details?id=com.darshancomputing.alockblock">A
Lock Block</a>.  Please see <a
href="https://github.com/darshan-/A-Lock-Block-Support/blob/master/FAQ.wiki#why-did-you-pull-this-functionality-out-of-batterybot-pro">that
project's FAQ</a> for why I made the decision to do this.

v8.3.5
 * Added link to Google Plus Page: https://www.google.com/+BatterybotInfoAndroid (follow
   for announcements and polls)
 * Try not to crash if storage is full (for example, when logging an event or adding an alarm)

v8.3.4
 * Better experience on most devices when first upgrading to Lollipop
   by setting Use System Layout to true.  You can turn it back to
   false if you prefer.
 * Fix crash on older devices when closing Service while large desktop widget present.
 * Fix crash when rotating screen while dialog present on History screen
 * Apply log filters immediately for consistency and correctness
 * Significantly updated Russian translations

v8.3.3

 * Better handling of Android's phantom-widget bug: the Service is now
 always closeable, and widgets appropriately reflect when they are
 disconnected from the Service.
 * Show Filter and Reverse Order menu items on ActionBar (in History) even on phones.
 * Enable fast scrolling in History

v8.3.2

 * Modern look for alarm overview page
 * Modern alarm notification icon on modern devices
 * Show Settings and Help menu items on ActionBar even on phones
 * Resolve several rare crashes reported on Developer Console
 * Added missing menu hint on two settings pages for pre-ICS devices

v8.3.1

 * Added an option on Lollipop devices using the Classic icon set to
   force the old color mode, since users reported that some devices on
   Lollipop do in fact support colored notification icons.

v8.3.0

 * Fixed the Classic icon set on Android 5.0+.  It will now display as
   only white and transparent, as required by Android.  Please see the
   <a href="https://github.com/darshan-/Battery-Indicator-Support/blob/master/FAQ.wiki#Why_does_the_Classic_icon_set_display_only_in_white_on_Android_50_Lollipop_and_later">FAQ</a> for more info.
 * Added frequently-requested support for milliamp information on
  supported devices.  Please see the
   <a href="https://github.com/darshan-/Battery-Indicator-Support/blob/master/FAQ.wiki#why-doesnt-the-current-ma-show-up-by-default--why-doesnt-it-work-on-my-device">FAQ</a> for more info.

v8.2.3

 * Fixed user-reported bug: App would crash if battery status changed while scrolling through history
 * Fixed rare Android-reported bug involving history menu
 * Updated Japanese translations

v8.2.2

 * Added Japanese translations

v8.2.1

 * Updated notifications to be visible on Lollipop (Android 5.0+) secure lockscreens.

v8.2.0

 * Updated app for Android 5.0 Lollipop.

 * Updated Turkish translations.

v8.1.10

 * Several fixes for rare crashes reported in Developer Console.

 * Minor performance improvement when viewing logs.

v8.1.9

 * Fix for rare crash reported in Developer Console.

v8.1.8

 * Updated widget appearance based on frequent user feedback.

 * Updated German translation.

v8.1.7

 * Added some lower temperature thresholds for high-temperature alarm, per user request.

 * Extensive updates to Arabic translation, substantial updates to German and Hungarian translations, small update to Polish translation.

v8.1.6

 * Changed app launcher icon to better match the rest of app.

 * Changed appearance of help screens to better match the rest of app.

 * Updated main help page with new links; removed outdated or redundant information.

 * Initial Arabic translation.

v8.1.5

 * Bugfix: The large widget would sometimes get out of sync.

 * Updated German translation.

 * Updated contact info.

v8.1.4

 * Updated German translation.

v8.1.3

 * Fixed missing string in Polish translation that caused crash when app run in Polish.

v8.1.2

 * Added a new, larger widget with more information.

 * Significant updates to Polish translation.

v8.1.1

 * The notification is now optional.  If you prefer to only use the app widget (or if you only like to check the app periodically and don't want the notification), you can now hide the notification from the main menu.

 * The app will no longer let you close the service if you have any widgets running. (If you have any pre-existing widgets from the previous release, this won't take effect until the next device restart.)

v8.1.0

 * This release adds a basic 1x1 circle widget. I plan to make it very configurable for Pro users. I also plan to add larger widget styles including the battery image and time-remaining estimate, etc.

 * NOTE: For now, you MUST leave the app running for the widget to work. I plan to fix this very soon, so that you will be able to have just the widget without the notification if you like.

 * Updated Dutch translations.

v8.0.10

 * New option to select the algorithm for the time-remaining estimates. Choose from "Sensitive" (the old default), "Conservative" (the current default since v8.0.9), "Since Status Change", or "Long-term Average". Find this option under "Other Settings".

 * Minor bugfixes.

 * Removed the "Beta" label. Help test out new features before they're released by joining the beta program: https://plus.google.com/communities/108365502089038835850

v8.0.9 (Beta)

 * The time-remaining estimates are now less sensitive. They're still based on recent usage, but you won't get the dramatic swings you had before. I plan to add back the old algorithm as an option for Pro users very soon. In the meantime, please let me know what you think of the estimates.

 * _Bugfix_: When charging past 100%, the estimates would count backwards until Fully Charged.

 * _Bugfix_: Disabling or enabling logging now takes effect immediately.

 * Updated Spanish translations.

v8.0.8 (Beta)

 * _Bugfix_: Last release included a regression where very first run of clean install would cause a force close.

v8.0.7 (Beta)

 * Many subtle bugs fixed.  If you've noticed any strange or incorrect behavior with alarms, time-remaining estimates, or time since status changed, this should (hopefully) fix things for you.  As always, please let me know if you run into any problems.

v8.0.6 (Beta)

 * Added ability to set custom colors for the notification, rather than just choosing among a few pre-set color options.

 * Made the time-remaining estimates handle rare conditions better. I'm hoping this will resolve the issues a few people have been reporting about seeing estimates of 0 minutes or several hundred days. Please contact me if you have any other issues around this!

 * Fairly substantial updates to both Dutch and Italian translations.

v8.0.5 (Beta)

 * Added an option to use the system notification layout, since the custom layout doesn't fit in on some devices.

v8.0.4 (Beta)

 * The notification in the drop down tray is now extremely configurable, both in what it shows and how it shows it.
 * Exporting history / logs to CSV now includes both Fahrenheit and Celsius.
 * Updated Hungarian translations.

v8.0.3 (Beta)

 * Due to many complaints about the notification being too cluttered and not lining up properly with other notifications on Honeycomb+, I've cleaned things up by removing the battery graphic and fixing the alignment to be consistent with the default notification layout. More notification configuration options will be coming soon for Pro users.
 * Updates to German, Romanian, and Russian translations.
 *  Minor fixes.

v8.0.2 (Beta)
 * Added option to show time since last status change rather than estimate of time remaining.
 * _Bugfix_: Fixed option to disallow use of disable lockscreen button, which was broken in redesign.

v8.0.1 (Beta)
 * _Bugfix_: App was restarting itself shortly after being closed.
 * _Bugfix_: Jellybean notification priority setting was accidentally disabled even on Android 4.1+.
 * _Bugfix_: Service is sometimes called with null Intent on some devices, which I hadn't thought possible, causing a crash.

v8.0.0 (Beta):

 * Initial release of !BatteryBot Pro.
 * Complete redesign of notification and main interface.
 * Fully automatic time remaining estimates based on recent usage.
 * Significantly reduced memory usage for the Service.
 * Lots of changes under the hood and groundwork laid for upcoming features.

v7.0.6
 * Efficiency improvements to Motorola one-percent mode.
 * Made Service less likely to be killed, which should result in increased accuracy and performance, especially on devices with a task killer.

v7.0.5
 * Automate one-percent hack.  (It will be used if possible, and the option to turn it on/off has been removed.)  Please let me know if you notice anything strange or get any crashes.
 * Automatically restart the service after an upgrade (uses *Autostart at Boot* setting).

v7.0.4
 * Added time deltas to logs.  (Major status changes show how long since plugged in / unplugged).
 * _Bugfix_: Finally fixed long-standing issue where, on Android 3.0+, disabled lock screen (a.k.a. keyguard) would become reenabled if a notification is pressed.
 * _Bugfix_: Fixed bug where the app would crash if the screen was turned off while viewing the logs.

v7.0.3
 * Added filters to logs (you can exclude status types that you aren't interested in).
 * Removed `log_everything` setting -- the new log filtering feature makes this option pointless.
 * Don't trigger `charge_rises` alarm if status is unplugged.  (You probably only care if you've _charged_ above your threshold, not if there's a minor fluctuation while discharging at your threshold.)
 * Significant updates to Dutch translation; some minor updates to several other translations.

v7.0.2
 * Fixed layout issue a small minority of devices were having with the Alarms screen.
 * Added new health status: "Cold".
 * Added new charging status: "Wireless".

v7.0.1
 * Updated launcher icon.  (Sorry for updating so soon for something so minor, but the new icon got pushed out with the update to Free, and I don't want Free having a better icon than Pro.)

v7.0.0
 * There are now three built-in icon sets, and the default set for Android 3.0+ (Honeycomb and newer) is now even larger than before.  The default set on older devices is the old classic set.  On the few newer devices that don't actually shrink and dim the icons, or don't do so as much as stock Android, you might prefer to select the smaller white number or the old classic set.  Plugins are still supported.
 * The newer sets with the plain number and charging indicator now make the charging indicator optional.
 * _Translations_: Added Slovenian translations.
 * _Translations_: Updated Hungarian translations.
 * Unified build process to make updates easier; removed support for API levels 3 and 4 (Android 1.5 / Cupcake and Android 1.6 / Donut) for this version forward to make this work.  The old version will continue to work for this 0.4% of users.
 * Removed !BackupAgent, at least for now, as it seemed to cause as many problems as it solved.

v6.0.3
 * This update provides a *possible* fix for users who were having trouble with the alarms. Since I don't have one of the devices with the problem, it's hard to know. If you have been having trouble with the alarms, please send me an email letting me know if this update helped or not. Thanks!

v6.0.2
 * Show separate notification when the lock screen is being disabled by the app. This can be turned off if desired.
 * Users of Jelly Bean (Android 4.1+) can set the notification priority. Set to "minimum" to hide the icon while leaving the notification in the tray. Defaults to "low" to lower the notification in the tray to allow other notifications to be more easily accessed. Set to "default" (which is Android's default, not Battery Indicator's) for normal behavior.
 * Now only displays the voltage if the reported voltage is realistic. Some devices (e.g. Nexus 7) report an invalid voltage that is no longer displayed.
 * Make the main window action bar a brighter, more noticeable gray

v6.0.1
 * Users of Android 3.0+, who have the plain number icon by default, now have a translucent rather than black icon background, due to many user requests. Don't forget you can still get the classic icons as a plugin.
 * Fixed bug with auto-disable lockscreen feature where the lockscreen would become disabled unexpectedly after first unlocking if it was never unlocked while plugged in.
 * Fixed bug in Dutch translations (my fault, not the translator's) that caused the alarms to malfunction.  (Dutch users, please let me know if you still have any problems.)
 * Minor update to Dutch translations and major update to Polish translations.

v6.0.0
 * Users of Honeycomb (Android 3.0), Ice Cream Sandwich (Android 4.0), and up now have a different default icon set that is much easier to see on these devices.  NOTE: This only changes which icon set is used by default -- as Pro users, you can always get the new icons on an older device, or still use the old colored icons on a newer device.
 * Disabled timestamp in notification by default; added an option to reenable it.
 * Updated French, Italian, and Traditional Chinese translations.

v5.1.5
 * Added initial Lithuanian translation.
 * Updated Greek translation.

v5.1.4
 * Added complete Greek translation.
 * Fairly large update to Dutch translation.
 * Minor updates to most other translations.

v5.1.3
 * Fixed error in Brazilian Portuguese translation that was causing a force close.

v5.1.2
 * Updated Dutch and Turkish translations.
 * Clarified some help text.
 * Show percentage sign with Textual charge level feature.

v5.1.1
 * _Bugfix_: Triggered alarms were not being shown if you used an icon plugin.  They should now work perfectly with or without icon plugins.

v5.1.0
 * Updated Slovak translation.
 * Improved appearance on Droid X (and possiblity other, similar devices).
 * Long-awaited experimental single-percent increments for most devices that previously only showed ten-percent increments.  Please see [http://code.google.com/p/battery-indicator/wiki/OnePercentHack?tm=6 OnePercentHack] for more info, and to report your results.

v5.0.7
 * Updated translations (in particular, the long-standing German landend/ladend issue).
 * Disable 'colorful small' window theme.
 * Minor layout fix.

v5.0.6
 * Fixed full screen window theme so that the app completely fills the screen again.

v5.0.5
 * Improved support for Android 4.0 (Ice Cream Sandwich) for Galaxy Nexus.
 * Minor layout fixes.

v5.0.4
 * Fix for a technical matter forgotten in 5.0.3 release.

v5.0.3
 * Updated Romanian, Russian, and Brazilian Portuguese translations.
 * Minor layout fixes.

v5.0.2
 * Layout fixes for most translations.

v5.0.1
 * Fixed Russian translation (it was causing a force-close for Russian-language users).

v5.0.0
 * New Feature: Icon plugins. There are just a few plugins right now, but they are very useful for black status bars, and more plugins will be coming.
 * There are also quite a few translation updates and several new translations.

v4.0.4
 * Avoid force closing on devices that don't have !BackupManager.

v4.0.3
 * Add !BackupManager support for devices that use it.
 * Update contact info and website URLs.

v4.0.2
 * Re-enable Cupcake support.

v4.0.1 (_Translations_)
 * Due to a bug in the web translation interface, many languages lost a few important translations.  The bug is now fixed, and the translations are back in this release.
 * Updated French and Italian translations.

v4.0.0
 * Initial support for Honeycomb tablets. There are more tablet optimizations planned, but this is a good start.
 * Several updated translations.
 * Automatically detect when preference summaries use a Formatter; removed manual configuration option so users don't have to deal with this.  It should "just work" now.
 * Unfortunately, I had to remove Cupcake (Android 1.5) support in order to add Honeycomb support. The reasons are complicated, annoying, and out of my control. Cupcake users can still use the previous version.

v3.1.5 (_Translations and Bugfix_)
 * Initial Czech, Hungarian, and Slovak translations.
 * Fix a Force Close bug that might have happened when connecting certain car chargers, and possibly in other situations.

v3.1.4 (_Translations_)
 * Initial French translations.

v3.1.3 (_Translations_)
 * Fixed Chinese translations for Hong Kong users

v3.1.2 (_Bugfix_)
 * This release provides a workaround for a bug in !CyanogenMod. If you use !CyanogenMod and get a Force Close when editing certain Battery Indicator settings, after upgrading you should go to Other Settings (in this app) and select the setting for *Summaries Use Formatter*.

v3.1.1 (_Bugfix_)
 * Someone managed to put a _null_ String in a place I thought one couldn't show up.  Fixed now.

v3.1.0
 * Alarms: With the new alarm feature, the app can now notify you when your battery becomes full, when the charge drops below or rises above a chosen level, if the temperature rises above a chosen level, or if the battery health fails.
 * (_Translation_) Partial French translations.
 * (_Translation_) Updated Italian translations.
 * (_Translation_) Fix error in Simplified Chinese translations.

v3.0.6 (_Translations_)
 * (_Translation_) Add Italian translations.

v3.0.5 (_Translations_)
 * (_Translation_) Fix Traditional Chinese translations.

v3.0.4 (_Translations_)
 * (_Translation_) Add Spanish translations.
 * (_Translation_) Add Traditional Chinese translations.

v3.0.3
 * (_Bugfix_) Remove FLAG_ACTIVITY_RESET_TASK_IF_NEEDED from Intent used to launch Battery Use screen. It doesn't appear to be necessary, and it caused a problem on at least one user's phone (which is a Droid X, but don't know if that's relevant).
 * (_Bugfix_) Some phones fluctuate wildly in their reported charge.  This causes Battery Indicator to think either that the phone has been charged or that a fuller battery has been put in.  I've adjusted the threshold to hopefully work well both for those with phones that fluctuate and for those who carry spare batteries.  With this version, a jump of 30 points or more is guaranteed to trip the switch, while a jump of 20 points or fewer is guaranteed not to. (For 21-29, it just depends on the situation).
 * (_Translation_) Add Chinese translations.

v3.0.2 (_Bugfix_)
 * (_Bugfix_) Auto-disable keyguard properly: User has to manually dismiss the keyguard once, then it will be disabled. This is both more secure (for secure screen locks) and fixes a bug that was present in various forms with all screen locks (including 'None').
 * (_Bugfix_) Make sure database is always closed properly.

v3.0.1
 * Log temperature and voltage, too.
 * Ability to export logs to CSV on SD card.
 * Option to close main window immediately after launching Battery Use screen.
 * Option to disallow manual lock screen disable.
 * A handful of minor tweaks and improvements throughout.

v3.0.0
 * Estimated discharge / charge time left. (Optional)
 * Logging of battery state. (Optional)
 * Themes for the main window. (Optional)
 * Manually/automatically dis/reenable the device lock screen. (Optional)
 * Efficiency improvements throughout.
 * Actually _smaller_ despite all the new features.
 * A "soft reset" of the service when you change settings, so the icon doesn't blink.
 * Green down to 20% (previous limit was 30%).
 * It now notices if a fuller battery has been put in, or if the phone was charged while off.
 * Trimmed down interface, moving many things to a menu.
 * So many new settings that they've been broken into multiple, easier to use pages.
 * Help pages explaining all of the settings.
 * Option to show the charge as larger text (only in notification tray).
 * Color preview.

<a name="free-version">
## Free Version

v11.0.3

 * Disabled notification badge by default for main channel.
 * Updated build tools.
 * Updated target audience.

v11.0.2

 * Fixed problem with widget-only mode (no notification) on 8.0+ devices (XX%).

v11.0.1

 * Brought classic color mode back, since some devices still support it on current versions of Android (Samsung seems to, at least).
 * Raised default priority for main Notification Channel (brings icon back to status bar by default) on Pre-9.0 versions of Android.
 * Initial Hindi and Farsi translations.

v11.0.0

 * Support for Android 8.0, 8.1, and 9.0 (Oreo and Pie), particularly Notification Channels.
 * Several bugfixes, mostly minor.
 * Efficiency improvements.
 * Initial Hebrew and Serbian translations.

v10.0.1

 * Bugfix: Remove timestamp from main notification

v10.0.0
 * Support Android 6.0+ (Marshmallow) and Android 7.0+ (Nougat), including split-screen view
 * Many significant improvements in performance, stability, and memory efficiency
 * Notification Wizard: makes it easier to adjust how notification is shown, adds feature
   previously only for Pro users to hide task bar icon but keep notification (requires Android 4.1+)
 * Updated Japanese and Chinese translations
 * Add privacy policy
 * Use Fahrenheit by default for en-US and es-US locales
 * Check for notifications being blocked, warn user and link to settings to unblock
 * Remove use_system_layout option; always use system layout now
 * Many minor fixes

v9.0.1

* Fix bug where app wouldn't always close when Close selected from menu (e.g. after rotation).
* Fix bug where 1x1 circle widget showed up as 2x2 on some launchers.
* Make circle widget the same size as a launcher icon, even when the desktop grid gives
  it more space than that.
* Removed shadow from below battery graphic in main screen, which was not noticeable on most devices
  but looked ugly where it was noticeable.
* Added xxxhdpi launcher icon.
* Don't show redundant 'Fully Charged' in the prediction (time remaining) area of the main screen,
  but rather indicate with an mdash that there is currently no prediction.
* Updated traditional Chinese translations.
* Removed shadow from below battery in launcher icon.

v9.0.0

* Redesigned main screen to look better, be easier to find the
  information you're looking for, and provide more information.

v8.3.5
 * Added link to Google Plus Page: https://www.google.com/+BatterybotInfoAndroid (follow
   for announcements and polls)

v8.3.4
 * Better experience on most devices when first upgrading to Lollipop
   by setting Use System Layout to true.  You can turn it back to
   false if you prefer.
 * Significantly updated Russian translations

v8.3.3

 * Better handling of Android's phantom-widget bug: the Service is now
 always closeable, and widgets appropriately reflect when they are
 disconnected from the Service.

v8.3.2

 * Show Settings and Help menu items on ActionBar even on phones
 * Resolve several rare crashes reported on Developer Console

v8.3.1

 * Added an option on Lollipop devices using the Classic icon set to
   force the old color mode, since users reported that some devices on
   Lollipop do in fact support colored notification icons.

v8.3.0

 * Fixed the Classic icon set on Android 5.0+.  It will now display as
   only white and transparent, as required by Android.  Please see the
   <a href="https://github.com/darshan-/Battery-Indicator-Support/blob/master/FAQ.wiki#Why_does_the_Classic_icon_set_display_only_in_white_on_Android_50_Lollipop_and_later">FAQ</a> for more info.

v8.2.3

 * Updated Japanese translations

v8.2.2

 * Added Japanese translations

v8.2.1

 * Updated notification to be visible on Lollipop (Android 5.0+) secure lockscreens.

v8.2.0

 * Updated app for Android 5.0 Lollipop.

 * Updated Turkish translations.

v8.1.10

 * Fix for rare crash reported in Developer Console.

v8.1.8

 * Updated widget appearance based on frequent user feedback.

 * Updated German translation.

v8.1.7

 * Extensive updates to Arabic translation, substantial updates to German and Hungarian translations, small update to Polish translation.

v8.1.6

 * Changed app launcher icon to better match the rest of app.

 * Changed appearance of help screens to better match the rest of app.

 * Updated main help page with new links; removed outdated or redundant information.

 * Initial Arabic translation.

v8.1.5

 * Bugfix: Rare widget synchronization issue.

 * Updated German translation.

 * Updated contact info.

v8.1.4

 * Updated German translation.

v8.1.3

 * Fixed missing string in Polish translation that caused crash when app run in Polish.

v8.1.2

 * Significant updates to Polish translation.

v8.1.1

 * This release adds a basic 1x1 circle widget. I plan to make it very configurable for Pro users. I also plan to add larger widget styles including the battery image and time-remaining estimate, etc. for Pro.

 * The notification is now optional. If you prefer to only use the app widget (or if you only like to check the app periodically and don't want the notification), you can now hide the notification from the main menu.

 * Updated Dutch translations.

v8.1.0  (_Skipped in free version_)

v8.0.10

 * Minor bugfixes.

 * Removed the "Beta" label. Pro users can help test out new features before they're released by joining the beta program: https://plus.google.com/communities/108365502089038835850

v8.0.9 (Beta)

 * The time-remaining estimates are now less sensitive. They're still based on recent usage, but you won't get the dramatic swings you had before. I plan to add back the old algorithm as an option for Pro users very soon. In the meantime, please let me know what you think of the estimates.

 * _Bugfix_: When charging past 100%, the estimates would count backwards until Fully Charged.

 * Updated Spanish translations.

v8.0.8 (Beta)

 * _Bugfix_: Last release included a regression where very first run of clean install would cause a force close.

v8.0.7 (Beta)

 * Many subtle bugs fixed.  If you've noticed any strange or incorrect behavior with time-remaining estimates or time since status changed, this should (hopefully) fix things for you.  As always, please let me know if you run into any problems.

v8.0.6 (Beta)

 * Made the time-remaining estimates handle rare conditions better. I'm hoping this will resolve the issues a few people have been reporting about seeing estimates of 0 minutes or several hundred days. Please contact me if you have any other issues around this!

 * Updates to both Dutch and Italian translations.

v8.0.5 (Beta)

 * Added an option to use the system notification layout, since the custom layout doesn't fit in on some devices.
 * Updated Hungarian translations.

v8.0.4 (Beta) (_Skipped in free version_)

v8.0.3 (Beta)

 * Due to many complaints about the notification being too cluttered and not lining up properly with other notifications on Honeycomb+, I've cleaned things up by removing the battery graphic and fixing the alignment to be consistent with the default notification layout. More notification configuration options will be coming soon for Pro users.
 * Updates to German, Romanian, and Russian translations.
 *  Minor fixes.

v8.0.2 (Beta)
 * Added option to show time since last status change rather than estimate of time remaining.

v8.0.1 (Beta)
 * _Bugfix_: App was restarting itself shortly after being closed.
 * _Bugfix_: Service is sometimes called with null Intent on some devices, which I hadn't thought possible, causing a crash.

v8.0.0 (Beta)

 * Initial release of !BatteryBot.
 * Complete redesign of notification and main interface.
 * Fully automatic time remaining estimates based on recent usage.
 * Significantly reduced memory usage for the Service.
 * Lots of changes under the hood and groundwork laid for upcoming features.

v7.0.6
 * Efficiency improvements to Motorola one-percent mode.
 * Made Service less likely to be killed, which should result in increased accuracy and performance, especially on devices with a task killer.
 * Fix for wireless charging.

v7.0.5
 * Automate one-percent hack.  (It will be used if possible, and the option to turn it on/off has been removed.)  Please let me know if you notice anything strange or get any crashes.
 * Automatically restart the service after an upgrade (if it was running).

v7.0.4
 * Removed some unnecessary strings.

v7.0.3
 * Significant updates to Dutch translation; some minor updates to several other translations.

v7.0.2
 * Added new health status: "Cold".
 * Added new charging status: "Wireless".

v7.0.1
 * There are now three built-in icon sets, and the default set for Android 3.0+ (Honeycomb and newer) is now even larger than before.  The default set on older devices is the old classic set.  On the few newer devices that don't actually shrink and dim the icons, or don't do so as much as stock Android, you might prefer to select the smaller white number or the old classic set.
 * _Translations_: Added Slovenian translations.
 * _Translations_: Updated Hungarian translations.
 * Unified build process to make updates easier; removed support for API levels 3 and 4 (Android 1.5 / Cupcake and Android 1.6 / Donut) for this version forward to make this work.  The old version will continue to work for this 0.4% of users.
 * Updated launcher icon.

v6.0.2
 * Now uses notification prioriy "low" on Jelly Bean (Android 4.1+) to lower the notification in the tray to allow other notifications to be more easily accessed.
 * Now only displays the voltage if the reported voltage is realistic. Some devices (e.g. Nexus 7) report an invalid voltage that is no longer displayed.
 * Make the main window action bar a brighter, more noticeable grey.

v6.0.1
 * Users of Android 3.0+, who have the plain number icon by default, now have a translucent rather than black icon background, due to many user requests.
 * Minor update to Dutch translations and major update to Polish translations.
 * Increased major version number to stay synchronized with Pro version.

v5.0.0
 * Users of Honeycomb (Android 3.0), Ice Cream Sandwich (Android 4.0), and up now have a different icon set that is much easier to see on these devices.
 * Disabled timestamp in notification.
 * Updated French, Italian, and Traditional Chinese translations.

v4.1.3
 * Added initial Lithuanian translation.
 * Updated Greek translation.

v4.1.2
 * Added complete Greek translation.
 * Updated Dutch translation.

v4.1.1
 * Updated Dutch and Turkish translations.
 * Clarified some help text.
 * Show percentage sign with Textual charge level feature.
 * Simplified settings screen.

v4.1.0
 * Updated Slovak translation.
 * Long-awaited experimental single-percent increments for most devices that previously only showed ten-percent increments.  Please see [http://code.google.com/p/battery-indicator/wiki/OnePercentHack?tm=6 OnePercentHack] for more info, and to report your results.

v4.0.8
 * Updated translations (in particular, the long-standing German landend/ladend issue).
 * Improved support for Android 4.0 (Ice Cream Sandwich).
 * Minor layout fixes.

v4.0.7
 * Updated Romanian, Russian, and Brazilian Portuguese translations.

v4.0.6
 * Fixed Russian translation (it was causing a force-close for Russian-language users).

v4.0.5
 * Many new and updated translations.

v4.0.4
 * Update contact info and website URLs.

v4.0.3
 * Backport option from Pro version to add textual charge level to notification.  This is easier for some people to see and critically important for those using a screen reader to interact with their device.

v4.0.2
 * Reduce package size by 35%.

v4.0.1
 * Re-enable Cupcake support.

v4.0.0
 * Initial support for Honeycomb tablets. There are more tablet optimizations planned, but this is a good start.
 * Several updated translations.
 * Unfortunately, I had to remove Cupcake (Android 1.5) support in order to add Honeycomb support. The reasons are complicated, annoying, and out of my control. Cupcake users can still use the previous version.

v3.0.6 (_Translations and Bugfix_)
 * Initial Czech, Hungarian, and Slovak translations.
 * Fix a Force Close bug that might have happened when connecting certain car chargers, and possibly in other situations.

v3.0.5 (_Translations_)
 * Updated French translations.

v3.0.4 (_Translations_)
 * French translations
 * Improved Italian translations
 * Fixed Chinese translations for Hong Kong users

v3.0.3 (_Translations_)
 * (_Translation_) Add Italian translations.

v3.0.2 (_Translations_)
 * (_Translation_) Add Spanish translations.
 * (_Translation_) Add Traditional Chinese translations.

v3.0.1
 * (_Bugfix_) Remove FLAG_ACTIVITY_RESET_TASK_IF_NEEDED from Intent used to launch Battery Use screen. It doesn't appear to be necessary, and it caused a problem on at least one user's phone (which is a Droid X, but don't know if that's relevant).
 * (_Bugfix_) Some phones fluctuate wildly in their reported charge.  This causes Battery Indicator to think either that the phone has been charged or that a fuller battery has been put in.  I've adjusted the threshold to hopefully work well both for those with phones that fluctuate and for those who carry spare batteries.  With this version, a jump of 30 points or more is guaranteed to trip the switch, while a jump of 20 points or fewer is guaranteed not to. (For 21-29, it just depends on the situation).
 * (_Translation_) Add Chinese translations.

v3.0.0
 * Easy access to the system's Battery Use screen (requires Android 1.6+).
 * Hi-res icons (requires hi-res device).
 * A couple of new settings.
 * Efficiency improvements throughout.
 * It now notices if a fuller battery has been put in, or if the phone was charged while off.
 * Trimmed down interface, moving many things to a menu.
 * Help page explaining the settings.
