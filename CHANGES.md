# Version 1.?.? - 2017-??-??
 * i18n: Serbian translation
 * i18n: Updated translations for Esperanto and Portuguese (Brazil)

# Version 1.0.1 - 2017-03-26
 * recording: Use H.264 baseline profile for MP4 for increased browser
              compatibility (#111)
 * recording: For WebM GNOME Shell recorder use same quality settings as with
              FFmpeg encoder
 * ui: Show only the most recent "file saved" notification to avoid spamming
       the desktop with notifications.
 * fix: Set temporary directory for ImageMagick
 * fix: Always launch with `GDK_BACKEND=x11` for Wayland
 * fix: Detect if global menus are disabled in Unity when running as
        Flatpak / Snap package
 * i18n: Updated translations for Arabic, Czech, Russian and Spanish
 * i18n: New translations for Basque and Esperanto
 * docs: Added Debian instructions to build custom package
 * docs: Added Snappy install instructions (development builds only)

# Version 1.0.0 - 2017-03-11
 * recording: Support GNOME Shell screencast DBus service. Allows recording
   under GNOME Shell with XWayland (#33)
 * recording: Support WebM and MP4 as output format (#73)
 * recording: Added option to not record mouse cursor
 * recording: Default frame rate is now 10fps
 * ui: Recording can be started / stopped via configurable keyboard shortcut (#23)
 * ui: Add `--start`, `--stop` and `--toggle` command line parameters to control
       the recording
 * ui: Add `--backend` command line parameter to manually choose recording
       backend (`gnome-shell`, `ffmpeg` or `avcodec` for now)
 * ui: Hide button label on small window width. Allows for smaller recording area.
 * misc: Use org.freedesktop.FileManager1 DBus service for launching file manager.
 * fix: Fixed a possible race condition that could lead to empty or broken files (#1)
 * fix: Moving Peek partially outside the visible area does no longer break the
        recording. Instead the recording area is clipped to the visible part (#64)
 * fix: Starting recording in maximized window relocated the window on Ubuntu Unity (#74)
 * fix: When canceling the file chooser also stop the background processing
        of the image (#96)
 * i18n: Many updated translations, with Czech, Dutch, German, Lithuanian,
         Polish and Swedish 100% completed
 * package: Peek is available from a Flatpak repository (#85)
 * package: Provide AppStream data
 * docs: Much improved README

# Version 0.9.1 - 2017-02-21
 * i18n: Fixed Czech, Croatian, Korean, Dutch and Chinese (Simplified) not getting installed

# Version 0.9.0 - 2017-02-20
 * ui: Fix problem of app menu not available on certain desktop configurations (#6)
 * ui: Fix display of desktop notifications on Ubuntu Unity (#55)
 * ui: Close button is displayed left on Ubuntu Unity (#67)
 * ui: Workaround for gray borders under unity (#11)
 * ui: Smaller border around recording area
 * recording: Add resolution downsampling option (#32)
 * recording: Minimal frame rate is now 1fps
 * recording: Smaller temporary files by using libx264rgb instead of huffyuv (#2)
 * recording: Support for avconf, if ffmpeg is unavailable (#56)
 * i18n: Chinese (Simplified) translation
 * i18n: Croatian translation
 * i18n: Czech translation
 * i18n: Dutch translation
 * i18n: Italian translation
 * i18n: Korean translation
 * i18n: Norwegian Bokmål translation
 * i18n: Portuguese (Brazil) translation
 * i18n: Swedish translation
 * fix: Fix possible crash when loading schema from local folder
 * fix: Fix temp file deletion warning
 * package: Peek is installable via [Ubuntu PPA](https://code.launchpad.net/%7Epeek-developers/+archive/ubuntu/stable)
 * docs: Update installation instructions
 * docs: Added FAQs

# Version 0.8.0 - 2016-10-25
 * ui: Change button text while rendering (#24)
 * ui: Add a `--version` command line argument
 * ui: Show file choose directly after recording stops. This way
       rendering and choosing the file take place in parallel (#30)
 * recording: Correctly scale recording area on HiDPI screens (#20)
 * i18n: Arabic translation
 * i18n: Catalan translation
 * i18n: French translation
 * i18n: Lithuanian translation
 * i18n: Polish translation
 * i18n: Portuguese (Portugal) translation
 * i18n: Russian translation
 * i18n: Spanish translation
 * i18n: Ukrainian translation
 * misc: Added generic name and sub category to desktop file
 * misc: Added uninstall target, so source installations can be uninstalled
   with `make uninstall` (#28)
 * fix: Fix DBus service file if installed to location other than `/usr` (#13)
 * fix: Locales not loaded if not installed to /usr due to missing locale path

# Version 0.7.2 - 2016-07-07
 * ui: Fixed window size not saved properly in Gtk 3.20 (#5)

# Version 0.7.1 - 2016-02-28
 * build: Fixed building with Gtk 3.14
 * build: Allow building with Gettext < 0.19 (disables localized .desktop file)

# Version 0.7.0 - 2016-02-26
 * ui: Moved record / stop button to header
 * ui: Show desktop notification after saving, with ability
   to open the file manager from there
 * ui: Use custom styling for recording area overlay
 * i18n: .desktop file gets translated

# Version 0.6.0 - 2016-01-28
 * ui: Removed unused auto save option from preferences dialog
 * fix: Try to always open the file manager, not the image viewer
 * general: Changed app id to com.uploadedlobster.peek due to the previous using
            the wrong domain name by default. This also resets existing settings.
 * i18n: Updated German translation

# Version 0.5.0 - 2016-01-09
 * ui: Remember last used save folder
 * ui: The default file name used is now a localized hidden setting
 * ui: If dark theme is preferred is now a hidden setting

# Version 0.4.0 - 2016-01-08
 * ui: Prefer dark theme, removed custom window background hack
 * ui: Persist window position and size
 * recording: Do not block UI during GIF post processing

# Version 0.3.0 - 2016-01-08
 * ui: Added a "New window" action to app menu
 * fix: If fallback app menu was used it was not clickable
 * fix: Fixed warning and crash if indicators where shown when closing a window
 * fix: Delay indicator no longer resizes small windows
 * fix: Leave recording state if ffmpeg cannot be started
 * fix: App menu on Unity showed "Unknown application name"
 * i18n: App menu and preferences title are now localized

# Version 0.2.1 - 2016-01-07
 * i18n: Setup gettext
 * fix: Fixed installation directory for locale files

# Version 0.2.0 - 2016-01-07
 * ui: Application logo
 * ui: Size indicator is shown longer after resizing stops
 * fix: Fixed window transparency not properly set on some systems
 * fix: About dialog could not be closed with close button
 * i18n: Integrated translation extraction into build
 * i18n: German translation

# Version 0.1.0 - 2016-01-05
 * Initial public release with basic functionality working
