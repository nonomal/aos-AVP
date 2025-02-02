# Nova Video Player changelog

<a id="v6.3.27"></a>
## [v6.3.27 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.27) - 2025-02-02

- fix crash on external ssa subtitles

[Changes][v6.3.27]


<a id="v6.3.26"></a>
## [v6.3.26 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.26) - 2025-02-01

- fix text subtitles not displayed sometimes
- synced with new crowdin translations

[Changes][v6.3.26]


<a id="v6.3.25"></a>
## [v6.3.25 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.25) - 2025-01-31

- align with next google play release


[Changes][v6.3.25]


<a id="v6.3.24"></a>
## [v6.3.24 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.24) - 2025-01-29

- fix UPnP video library disappearing sometimes


[Changes][v6.3.24]


<a id="v6.3.23"></a>
## [v6.3.23 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.23) - 2025-01-28

- enable passthrough for all since detection mechanism does not work for SPDIF (only works with HDMI)


[Changes][v6.3.23]


<a id="v6.3.22"></a>
## [v6.3.22 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.22) - 2025-01-22

- switch back to mediacodec for audio decoding with ffmpeg fallback when not in passthrough

Feedback expected from users using an Android TV TV set using stereo speakers (no AV receiver) and reporting great sound experience on AC3 or DTS and stereo downmix when using previous releases.


[Changes][v6.3.22]


<a id="v6.3.21"></a>
## [v6.3.21 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.21) - 2025-01-22

- release candidate for Google Play, amazon, and F-Droid

[Changes][v6.3.21]


<a id="v6.3.20"></a>
## [v6.3.20 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.20) - 2025-01-18

- real regression fix for not scanning external usb storage devices when adding files to external storage
- real fix for external & pgs subtitles stuck sometimes


[Changes][v6.3.20]


<a id="v6.3.19"></a>
## [v6.3.19 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.19) - 2025-01-18

- fix regression of not scanning external usb storage devices
- fix external subtitles stuck sometimes
- handle more subtitle position tag formats (e.g. `\{\\an8\}`)
- Android frame synchronization for smoother playback disabled by default pending some AV desync fix
- stability enhancements


[Changes][v6.3.19]


<a id="v6.3.18"></a>
## [v6.3.18 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.18) - 2025-01-12

- add more technical information on Android TV info playing tile (screen HDR capabilities and current mode, supported refresh rates and current one, HDMI receiver audio capabilities)
- better foreground state detection to not launch service if in background
- stability enhancements


[Changes][v6.3.18]


<a id="v6.3.17"></a>
## [v6.3.17 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.17) - 2025-01-09

- smoother video playback with new experimental Android frame synchronization (can be disabled in expert options)
- stability enhancements


[Changes][v6.3.17]


<a id="v6.3.16"></a>
## [v6.3.16 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.16) - 2025-01-05

- apply ITU-R BS.775-3 coefficients for stereo downmixing
- fix NFO relocation regression (long lasting)
- fix nova use as external player with kodi
- fix 7.1 stereo downmix
- fix filename containing "#" not playing with some network share protocols (sftp, sshj, webdavs)
- try to use jcifs internal nova library instead of device one if it exists

[Changes][v6.3.16]


<a id="v6.3.15"></a>
## [v6.3.15 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.15) - 2024-12-21

- stability enhancements
- smbj 0.14.0 upstep
- sshj 0.39.0 upstep
- 2025 android TV banners

[Changes][v6.3.15]


<a id="v6.3.14"></a>
## [v6.3.14 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.14) - 2024-12-13

- stability enhancements
- new experimental Android frame synchronization expert option to test if it improves playback fluidity


[Changes][v6.3.14]


<a id="v6.3.13"></a>
## [v6.3.13 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.13) - 2024-12-11

- true passthrough support of TrueHD and DTS:X on Fire stick 4k max 2023 -- requires nova encapsulation mode 1

[Changes][v6.3.13]


<a id="v6.3.12"></a>
## [v6.3.12 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.12) - 2024-12-10

- select proper dolby vision codec depending on profile
- fix wrong internal subtitle selection based on language regression

[Changes][v6.3.12]


<a id="v6.3.11"></a>
## [v6.3.11 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.11) - 2024-12-09

- fix SMB discovery with freebox NAS SMB server when using smbj
- center text subtitles
- resume scrape at last video scrape instead of restarting when scan is interrupted

Important note: due to limitations imposed by Google when switching to API 34, foreground processes have not been granted to nova for background video media information retrieval. This means that nova cannot scan videos in background and full scan needs to be performed when nova is in foreground.
Coping with this constraint required some intrusive modifications that could result in some regressions and debug: hence the pre-release tag. 

[Changes][v6.3.11]


<a id="v6.3.10"></a>
## [v6.3.10 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.10) - 2024-12-08

- support subtitles position SSA tags
- better video identification logic

Important note: due to limitations imposed by Google when switching to API 34, foreground processes have not been granted to nova for background video media information retrieval. This means that nova cannot scan videos in background and full scan needs to be performed when nova is in foreground.
Coping with this constraint required some intrusive modifications that could result in some regressions and debug: hence the pre-release tag.


[Changes][v6.3.10]


<a id="v6.3.6"></a>
## [v6.3.6 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.6) - 2024-11-22

- fix on pgs subtitles duration computation


[Changes][v6.3.6]


<a id="v6.3.5"></a>
## [v6.3.5 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.5) - 2024-11-20

- completed pgs subtitles support
- gfx subtitles display rework (no scaling and repositioning possible) relying on ffmpeg decoding
- fix cycling through subtitles list with keycode


[Changes][v6.3.5]


<a id="v6.3.4"></a>
## [v6.3.4 pre-release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.4) - 2024-10-25

- add pgs subtitles support
- upgrade to ffmpeg 7.1, dav1d 1.5.0
- disable by default use Android timely frame posting for smoother playback since it causes some playback issues


[Changes][v6.3.4]


<a id="v6.3.3"></a>
## [v6.3.3 pre-release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.3) - 2024-10-06

- smoother playback: use Android timely frame posting

Please report any regression in playback and seek related to this release.


[Changes][v6.3.3]


<a id="v6.3.2"></a>
## [v6.3.2 pre-release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.3.2) - 2024-09-25

- upgrade to ffmpeg 7.0.2
- add locale setting in nova for devices with restricted language support
- target SDK 34 to comply with Google API rules
- fix network shortcuts host check to accept FQDN with TLD larger than 6 characters

[Changes][v6.3.2]


<a id="v6.2.95"></a>
## [v6.2.95 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.95) - 2024-08-27

- stability enhancements


[Changes][v6.2.95]


<a id="v6.2.93"></a>
## [v6.2.93 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.93) - 2024-08-17

- rationalize Chinese language strings


[Changes][v6.2.93]


<a id="v6.2.92"></a>
## [v6.2.92 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.92) - 2024-08-17

- fix traditional Chinese getting English video descriptions [#1129](https://github.com/nova-video-player/aos-AVP/issues/1129)


[Changes][v6.2.92]


<a id="v6.2.91"></a>
## [v6.2.91 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.91) - 2024-08-16

- fix PIP not working anymore
- revert to ffmpeg 4.4.5 to avoid playback regressions
- add Brazilian language for TMDB video descriptions


[Changes][v6.2.91]


<a id="v6.2.90"></a>
## [v6.2.90 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.90) - 2024-07-07

- Other scraper issues fixed


[Changes][v6.2.90]


<a id="v6.2.89"></a>
## [v6.2.89 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.89) - 2024-07-07

- Fix several scraper crashes seen on sentry

[Changes][v6.2.89]


<a id="v6.2.88"></a>
## [v6.2.88 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.88) - 2024-06-29

- Fix none subtitle track not applied at resume


[Changes][v6.2.88]


<a id="v6.2.87"></a>
## [v6.2.87 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.87) - 2024-06-25

- Fix subtitles not found in some cases
- Fix default opensubtitles search in Chinese and Portuguese variants not set correctly
- Enhance opensubtitles search stability
- Use correct reference to opensubtitles.com instead of opensubtitles.org that was misleading in some translations
- Fix incorrect Chinese subtitle language naming reported in Video information view

[Changes][v6.2.87]


<a id="v6.2.86"></a>
## [v6.2.86 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.86) - 2024-06-22

- Google play release candidate


[Changes][v6.2.86]


<a id="v6.2.85"></a>
## [v6.2.85 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.85) - 2024-06-20

- Fix one case of scan in loop

[Changes][v6.2.85]


<a id="v6.2.84"></a>
## [v6.2.84 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.84) - 2024-06-17

- Switched back to previous sardine-android to fix webdav regressions
- Fixed subtitle track not applied on next episode with binge mode play mode
- Fix smbj rename

[Changes][v6.2.84]


<a id="v6.2.82"></a>
## [v6.2.82 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.82) - 2024-06-16

- Fix random subtitles being selected sometimes
- Bump commons-net to 3.11.1, jsch to 0.2.18, sentry to 7.10.0, sardine-android to 0.9


[Changes][v6.2.82]


<a id="v6.2.81"></a>
## [v6.2.81 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.81) - 2024-06-09

- Fix favorite lang/sub not applied in binge watching mode
- tmdb-java bump to 2.11.0


[Changes][v6.2.81]


<a id="v6.2.79"></a>
## [v6.2.79 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.79) - 2024-05-29

- Use jupnp 3.0.2 for UPnP stack instead of deprecated cling
- Fix regression in oauthDialog

/!\ Please test UPnP and report  any issue.


[Changes][v6.2.79]


<a id="v6.2.78"></a>
## [v6.2.78 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.78) - 2024-05-28

- Select correctly external track with video.mkv and video-PL.srt and preferred language is Polish
- Desugaring is mandatory for old android version to avoid NoClassDefFoundError (e.g. smbj) and some missing java classes on Android (e.g. java.time etc.)
- commons-net upstep to version 3.10.0


[Changes][v6.2.78]


<a id="v6.2.77"></a>
## [v6.2.77 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.77) - 2024-05-26

- More subtitle fixes on latest refactoring
- Stability enhancements


[Changes][v6.2.77]


<a id="v6.2.76"></a>
## [v6.2.76 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.76) - 2024-05-25

- Refactored subtitle selection logic: if external srt is present and no matching language is found it is selected
- Stability enhancements


[Changes][v6.2.76]


<a id="v6.2.75"></a>
## [v6.2.75 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.75) - 2024-05-19

- Fix default subtitle selection logic
- Some stability enhancements


[Changes][v6.2.75]


<a id="v6.2.74"></a>
## [v6.2.74 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.74) - 2024-05-12

- Revert from jupnp to cling because of errors seen on sentry


[Changes][v6.2.74]


<a id="v6.2.73"></a>
## [v6.2.73 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.73) - 2024-05-11

- Ugly fix to apply change of internal subtitle track (FIXME: it makes video seek)
- Simplify subtitle language detection based on filename analysis for external subtitle files


[Changes][v6.2.73]


<a id="v6.2.72"></a>
## [v6.2.72 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.72) - 2024-05-09

- Use jupnp 3.0.2 instead of cling for UPnP /!\ please report any issue with UPnP
- Many subtitles naming detection fixes
- Pass prefetched/local subtitles as files and not http URIs to external video players to fix encoding issues for JustPlayer
- Nova icon update for Google Play compliance


[Changes][v6.2.72]


<a id="v6.2.71"></a>
## [v6.2.71 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.71) - 2024-05-04

- Fix hide subtitles by default not working for internal subtitles regression
- More fixes for posters and trailer images not downloading on old Android version


[Changes][v6.2.71]


<a id="v6.2.70"></a>
## [v6.2.70 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.70) - 2024-04-28

- Fix hide subtitles by default not working regression
- Fix subs not passed to external video player
- Really fix posters not downloading on old Android version
- Now Android TV icon is compliant with Google Play requirements

[Changes][v6.2.70]


<a id="v6.2.69"></a>
## [v6.2.69 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.69) - 2024-04-19

- Fix poster download on old Android versions where system CA are outdated


[Changes][v6.2.69]


<a id="v6.2.67"></a>
## [v6.2.67 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.67) - 2024-03-30

- Fix notification icon

[Changes][v6.2.67]


<a id="v6.2.66"></a>
## [v6.2.66 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.66) - 2024-03-30

- Android TV icon update for Google Play compliance

[Changes][v6.2.66]


<a id="v6.2.65"></a>
## [v6.2.65 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.65) - 2024-03-19

- Fix sentry change of behavior reporting okhhtp3 50x error messages


[Changes][v6.2.65]


<a id="v6.2.64"></a>
## [v6.2.64 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.64) - 2024-03-15

- Add Android 12 match frame rate feature support for refresh rate selection (new mode in nova settings)
- Get back to EOL cling since jupnp not yet stable
- Subtitles fixes

[Changes][v6.2.64]


<a id="v6.2.63"></a>
## [v6.2.63 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.63) - 2024-02-18

- UPnP network shares: use jupnp Java library instead of EOL cling

Please report any issue with UPnP here [#74](https://github.com/nova-video-player/aos-AVP/issues/74)

[Changes][v6.2.63]


<a id="v6.2.62"></a>
## [v6.2.62 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.62) - 2024-02-17

- Unify scraper language settings 
- Global better ordering of language menus in settings
- Make Traditional Chinese appear in scraper languages
- Stability enhancements

/!\ This release will revert to default scrape language.


[Changes][v6.2.62]


<a id="v6.2.61"></a>
## [v6.2.61 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.61) - 2024-02-16

- Scrape shows and movies without air date reported by TMDB
- Remove deprecated old opensubtitles.org subs downloader
- Stability enhancements


[Changes][v6.2.61]


<a id="v6.2.59"></a>
## [v6.2.59 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.59) - 2024-02-15

- Stability enhancements


[Changes][v6.2.59]


<a id="v6.2.58"></a>
## [v6.2.58 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.58) - 2024-02-10

- Fix preferred audio language not applied
- Fix some remaining UI not responsible until back pressed on subs download in case of errors
- Stability enhancements


[Changes][v6.2.58]


<a id="v6.2.57"></a>
## [v6.2.57 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.57) - 2024-02-09

- Fix cannot download subs when logged in on opensubtitles.com
- Propose nova as external player when opening local files
- Stability enhancements

Note: this release does not contain the new jupnp UPnP client.

[Changes][v6.2.57]


<a id="v6.2.55"></a>
## [v6.2.55 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.55) - 2024-02-03

- Fix subtitles download for videos on UPnP shares
- Subtitles download stability enhancements


[Changes][v6.2.55]


<a id="v6.2.54"></a>
## [v6.2.54 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.54) - 2024-01-27

- Add preferred audio language option for multi audio track videos
- Prevent opensubtitles subtitles download when out of quota


[Changes][v6.2.54]


<a id="v6.2.53"></a>
## [v6.2.53 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.53) - 2024-01-20

- Handle webdav 302 redirect for real-debrid support
- Upstep jsch to 0.2.16, sshj to 0.38.0
- Stability enhancements


[Changes][v6.2.53]


<a id="v6.2.52"></a>
## [v6.2.52 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.52) - 2024-01-14

- Another attempt to fix ftp (please report if you experience issues)
- Stability enhancements


[Changes][v6.2.52]


<a id="v6.2.51"></a>
## [v6.2.51 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.51) - 2024-01-12

- libyuv upstep aligned on chromium master
- Stability enhancements


[Changes][v6.2.51]


<a id="v6.2.50"></a>
## [v6.2.50 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.50) - 2024-01-10

- Fix duplicate subs listed in VideoInfo for smbj shares


[Changes][v6.2.50]


<a id="v6.2.49"></a>
## [v6.2.49 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.49) - 2024-01-09

- Assume writeable directories on jcifs-ng
- Stability enhancements



[Changes][v6.2.49]


<a id="v6.2.48"></a>
## [v6.2.48 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.48) - 2024-01-08

- Fix F-Droid build
- Update Video information fragment if subtitles have been downloaded during playback or video has changed
- Fix more error found in play mode



[Changes][v6.2.48]


<a id="v6.2.47"></a>
## [v6.2.47 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.47) - 2024-01-07

- Cleaner Android TV years banner
- Better detect external subtitle language from filename
- Update Video information fragment if subtitles have been downloaded during playback
- Faster subtitle check on Android TV
- Fix an issue in play mode (folder mode fixed?)


[Changes][v6.2.47]


<a id="v6.2.46"></a>
## [v6.2.46 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.46) - 2024-01-05

- Fix various subtitles issues

[Changes][v6.2.46]


<a id="v6.2.44"></a>
## [v6.2.44 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.44) - 2024-01-03

- Bump ffmpeg to 6.1.1

[Changes][v6.2.44]


<a id="v6.2.43"></a>
## [v6.2.43 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.43) - 2024-01-03

- Handle properly gesture navigation screen layout in player UI


[Changes][v6.2.43]


<a id="v6.2.40"></a>
## [v6.2.40 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.40) - 2023-12-22

- Enforce new opensubtitles REST-API with quotas becoming mandatory in in January
- Disable gesture control when player screen is in locked mode
- New nova icon
- 2024 Android TV by year banners
- Attempt to support WebDAV 302 redirects
- Remember none subtitle track selection on resume
- Update boost to 1.84.0, libtorrent to 2.9.0
- Fix AV1 decoding regression
- Stability enhancements


[Changes][v6.2.40]


<a id="v6.2.38"></a>
## [v6.2.38 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.38) - 2023-11-27

- Gesture stability enhancements


[Changes][v6.2.38]


<a id="v6.2.37"></a>
## [v6.2.37 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.37) - 2023-11-26

- Add player gesture control
- Increase new opensubtitles REST-API downloader robustness

Following gestures are now supported:
- double tap on left/right regions of the screen for +-10s seek backward/forward
- scroll on left/right regions of the screen for brightness/volume increase/decrease

Two OSD regions have been added on top left/right screen part to display the fast rewind/forward icons and volume/brightness levels.


[Changes][v6.2.37]


<a id="v6.2.36"></a>
## [v6.2.36 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.36) - 2023-11-21

- New nova icon
- opensubtitles subtitles download based on REST-API stability enhancements
- Update smbj to 0.13.0, ffmpeg to 6.1, dav1d to 1.3.0

Please report any multimedia regression with ffmpeg 6.1 (e.g. AV1 is broken right now).

[Changes][v6.2.36]


<a id="v6.2.35"></a>
## [v6.2.35 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.35) - 2023-11-14

- Stability enhancements (crash on multi-selection subtitles download)
- Attempt to fix ftp on Android 7.1.2 devices cf. [#829](https://github.com/nova-video-player/aos-AVP/issues/829)

[Changes][v6.2.35]


<a id="v6.2.34"></a>
## [v6.2.34 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.34) - 2023-11-12

- New nova icon
- Add possibility to use new opensubtitles REST-API instead of XML-RPC that will be enforced in January
- Update jcifs-ng to 2.1.10, commons-net to 3.10.0, sshj to 0.37.0
- Add missing anime shows by alpha on Android TV
- Avoid top/bottom grey bars on chromebooks while playing videos

/!\ Please check new OpenSubtitles REST-API by activating it in nova settings and report any issue. OpenSubtitles will enforce use of this new API starting January 2024 and imposes download quotas (20 subs per day for a registered user, 5 otherwise). Note that you will need an opensubtitles.com account (and not an opensubtitles.org one)!


[Changes][v6.2.34]


<a id="v6.2.33"></a>
## [v6.2.33 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.33) - 2023-10-29

- Fix F-Droid checkupdates bot release pickup


[Changes][v6.2.33]


<a id="v6.2.32"></a>
## [v6.2.32 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.32) - 2023-10-15

- Update jcifs-ng to 2.1.10, commons-net to 3.10.0, sshj to 0.37.0

/!\ Please test if this release breaks ftp on firestick4k (not the max version) cf. [#829](https://github.com/nova-video-player/aos-AVP/issues/829)


[Changes][v6.2.32]


<a id="v6.2.31"></a>
## [v6.2.31 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.31) - 2023-10-10

- Fix hide subtitles by default not working regression
- Restore directories listed first when sorting by name

[Changes][v6.2.31]


<a id="v6.2.30"></a>
## [v6.2.30 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.30) - 2023-09-29

- Final design to only disable SMB UDP discovery to cope with Fire 10 HD Wi-Fi issues


[Changes][v6.2.30]


<a id="v6.2.29"></a>
## [v6.2.29 release candidate](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.29) - 2023-09-24

- Fix smbj not asking credentials when browsing an SMB server without guest account
- ffmpeg 4.4.4 upstep with DoVi patches
- dav1d 1.2.0 upstep
- openssl 1.1.1w upstep
- opus master upstep

[Changes][v6.2.29]


<a id="v6.2.28"></a>
## [v6.2.28 release candidate](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.28) - 2023-09-23

- Add an option to limit SMB discovery to mDNS disabling TCP/UDP discovery that makes Wi-Fi drivers on some devices (e.g. Fire 10 HD) to crash and turn off Wi-Fi. Note that TCP/UDP discovery is required for proper ChromeOS SMB discovery.

[Changes][v6.2.28]


<a id="v6.2.17"></a>
## [v6.2.17 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.17) - 2023-06-23

- Fix CI


[Changes][v6.2.17]


<a id="v6.2.16"></a>
## [v6.2.16 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.16) - 2023-06-22

- Attempt to solve voice search on Android 11 (shieldTV)
- Do not crash if tmdb backend has outage
- Add m3u support in manifest (TBC if it works)



[Changes][v6.2.16]


<a id="v6.2.15"></a>
## [v6.2.15 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.2.15) - 2023-06-18

- Fix A/V desync using playback speed
- Switched to jsch-mwiede fork for SFTP
- Use java 17


[Changes][v6.2.15]


<a id="v6.1.6"></a>
## [v6.1.6 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.1.6) - 2023-04-04

- Add tx3g (mov_text) subtitles support


[Changes][v6.1.6]


<a id="v6.0.97"></a>
## [v6.0.97 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.97) - 2023-02-12

- Fix ftp regression on some firesticks
- Stability enhancements


[Changes][v6.0.97]


<a id="v6.0.96"></a>
## [v6.0.96 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.96) - 2023-02-08

- Fix SMB1 regression on some NAS
- Perhaps fix F-droid not picking up new nova releases


[Changes][v6.0.96]


<a id="v6.0.95"></a>
## [v6.0.95 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.95) - 2023-02-04

- More subtitles shades of grey
- Stability enhancements


[Changes][v6.0.95]


<a id="v6.0.94"></a>
## [v6.0.94 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.94) - 2023-01-23

- Experimental playback speed option: fix subtitles not in sync and crash using bluetooth headsets
- Option to disable Dolby Vision decoder
- Pass list of subtitles to external video players



[Changes][v6.0.94]


<a id="v6.0.93"></a>
## [v6.0.93 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.93) - 2023-01-02

- Stability enhancements
- External player compatibility: mark video as watched with Just Player upon video completion
- Attempt to rework internal storage import service to avoid non visible crash in background


[Changes][v6.0.93]


<a id="v6.0.89"></a>
## [v6.0.89 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.89) - 2022-12-10

- Support more ssa subtitle style formats
- Fix SMB shortcut with empty user (guest) on AndroidTV
- 2023 banners for AndroidTV


[Changes][v6.0.89]


<a id="v6.0.88"></a>
## [v6.0.88 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.88) - 2022-11-29

- Target API33
- boost/libtorrent 1.80.0/2.0.8 upstep
- jcifs-ng SMB upstep to latest master
- Bundle delivery to Google Play
- Stability enhancements


[Changes][v6.0.88]


<a id="v6.0.87"></a>
## [v6.0.87 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.87) - 2022-11-21

- Fix infinite loop in refreshrate negotiation
- Stability enhancements


[Changes][v6.0.87]


<a id="v6.0.83"></a>
## [v6.0.83 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.83) - 2022-11-13

- Increase number of subtitles track supported to 64
- Stability enhancements


[Changes][v6.0.83]


<a id="v6.0.82"></a>
## [v6.0.82 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.82) - 2022-11-12

- Experimental playback speed option is back but disabled by default (could cause choppy video)
- Better movie scrape results through applying Levenshtein distance on tmdb scrape results
- Hidden advanced option to enable specifying lavc parser sync mode (PTS or sample)

[Changes][v6.0.82]


<a id="v6.0.81"></a>
## [v6.0.81 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.81) - 2022-11-08

- Re-disable experimental playback speed control due to instabilities

[Changes][v6.0.81]


<a id="v6.0.80"></a>
## [v6.0.80 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.80) - 2022-11-05

- Fix db update crash

[Changes][v6.0.80]


<a id="v6.0.79"></a>
## [v6.0.79 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.79) - 2022-11-05

- Crowdin translations synchronization
- Stability enhancements


[Changes][v6.0.79]


<a id="v6.0.76"></a>
## [v6.0.76 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.76) - 2022-10-26

- Disable experimental playback speed control for now since causes regressions


[Changes][v6.0.76]


<a id="v6.0.75"></a>
## [v6.0.75 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.75) - 2022-10-23

- Experimental playback speed control stability improvements (only when not using audio passthrough)
- Stability enhancements


[Changes][v6.0.75]


<a id="v6.0.71"></a>
## [v6.0.71 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.71) - 2022-06-23

**WARNING**: this v6 release of Nova consists in a major update compared to v5 and requires to rescan all video collection for multimedia information re-aquisition. It is strongly advised to restart from a clean install to avoid problems. Please check FAQ for details.

Incremental release changelog compared to previous v6 github release:
- Stability enhancements

v6 release changelog short summary compared to v5:

- Add support for movie collections/sagas on Android TV
- Separate section for animation movies and series on Android TV
- Switch to tmdb instead of tvdb for TV shows information retrieval
- Faster TV shows media information retrieval
- Fix crash on Android 12/S/API31
- Properly report DTS-HD and DTS-HD MA
- Dolby vision support
- ffmpeg 4.4.2 and dav1d 1.0.0 integration
- Add MDNS samba discovery
- New refresh rate selection algorithm optimizing judder effect
- Add domain option to samba network credential dialog
- Optimize network shares rescan speed in case of files delete/rename
- Binge watching play mode
- Display content rating and better audio/resolution tag on leanback
- STOP remote button stops player
- Add https streaming support
- Swedish, Greek, Traditional Chinese, Ukrainian translations in progress
- Add adult scrape hidden option NOT on google play
- Speed up initial local storage video import blacklisting whatsapp files before import
- Fix trakt tvshow sync
- Target API31 (warning: relocation of nfo/jpg for local storage videos
- Sentry crashnalytics backend integration
- Make animation row optional on android TV
- Add more blacklisted local storage directories to speed up media import
- Add possibility to exclude network shortcuts from automatic/scheduled/manual global rescans on Android TV
- Optimize launch time on Android TV 
- Fix youtube trailers not opening on youtube app on Android TV
- Add traditional Chinese, Brazilian, Ukrainian, Kurdish scrape/subs support
- Fix trakt multi-devices last played synchronization
- jcifs-ng SMB upstep
- SMB3 enabled by default (please test and report regressions!)
- Capability to add manual SMB shortcuts on ADTV
- 2022 year banners on ADTV
- Play button is first on tvshow all episodes view on ADTV
- Remove duplicate downmixing setting on phone/tablet UI
- Fix cannot play SMB file resulting from search result
- Stability enhancements

**More detailed migration notes:**

* This new version upgrades the internal nova media database to a new scheme and any downgrade to v4/v5 versions of nova will wipe out your entire video collection to prevent any incompatibility.
* This version switches to theMovieDb for retrieving TV shows information instead of theTvDb. It is strongly recommended to rescrape all your TV shows or start from a fresh install.
* Proper support for movie collections and animation movies/series on AndroidTV requires some manual steps. Acquisition of the additional movie collection informations and movies/TV series genres realignment requires a full rescrape of your video without interference of existing .nfo files (that do not yet contain the required information). For that purpose the following steps should do the trick:
    * backup all your customized handcrafted .nfo file (if you have any)
    * install nova version 6.xx
    * in nova settings unselect "process '.nfo' files"
    * in nova settings launch a "rescrape all" and wait for completion
    * in nova settings launch an "export already scraped videos" and wait for completion (**this step will override any existing .nfo file**)
* versions later than v6.0.30 targets API31 and due to Android storage restrictions for API30, local NFO/JPG media information files for videos stored on local storage have been moved to nova public application folder located /sdcard/Android/data/org.courville.nova/files/nfoPoster 
 * If you ever want to get back to nova v5.xx, you will need to clean application data *and cache*

[Changes][v6.0.71]


<a id="v6.0.70"></a>
## [v6.0.70 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.70) - 2022-06-21

- Play button is first on tvshow all episodes view on ADTV
- Remove duplicate downmixing setting on phone/tablet UI
- Fix cannot play SMB file resulting from search result
- Stability enhancements

[Changes][v6.0.70]


<a id="v6.0.67"></a>
## [v6.0.67 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.67) - 2022-06-05

**WARNING**: this v6 release of Nova consists in a major update compared to v5 and requires to rescan all video collection for multimedia information re-aquisition. It is strongly advised to restart from a clean install to avoid problems. Please check FAQ for details.

Incremental release changelog compared to previous v6 github release:
- Fix youtube trailers not opening on youtube app on Android TV
- Add traditional Chinese, Brazilian, Ukrainian, Kurdish scrape/subs support
- Fix trakt multi-devices last played synchronization
- jcifs-ng SMB upstep
- Stability enhancements

v6 release changelog short summary compared to v5:

- Add support for movie collections/sagas on Android TV
- Separate section for animation movies and series on Android TV
- Switch to tmdb instead of tvdb for TV shows information retrieval
- Faster TV shows media information retrieval
- Fix crash on Android 12/S/API31
- Properly report DTS-HD and DTS-HD MA
- Dolby vision support
- ffmpeg 4.4.2 and dav1d 1.0.0 integration
- Add MDNS samba discovery
- New refresh rate selection algorithm optimizing judder effect
- Add domain option to samba network credential dialog
- Optimize network shares rescan speed in case of files delete/rename
- Binge watching play mode
- Display content rating and better audio/resolution tag on leanback
- STOP remote button stops player
- Add https streaming support
- Swedish, Greek, Traditional Chinese, Ukrainian translations in progress
- Add adult scrape hidden option NOT on google play
- Speed up initial local storage video import blacklisting whatsapp files before import
- Fix trakt tvshow sync
- Target API31 (warning: relocation of nfo/jpg for local storage videos
- Sentry crashnalytics backend integration
- Make animation row optional on android TV
- Add more blacklisted local storage directories to speed up media import
- Add possibility to exclude network shortcuts from automatic/scheduled/manual global rescans on Android TV
- Optimize launch time on Android TV
- Stability enhancements

**More detailed migration notes:**

* This new version upgrades the internal nova media database to a new scheme and any downgrade to v4/v5 versions of nova will wipe out your entire video collection to prevent any incompatibility.
* This version switches to theMovieDb for retrieving TV shows information instead of theTvDb. It is strongly recommended to rescrape all your TV shows or start from a fresh install.
* Proper support for movie collections and animation movies/series on AndroidTV requires some manual steps. Acquisition of the additional movie collection informations and movies/TV series genres realignment requires a full rescrape of your video without interference of existing .nfo files (that do not yet contain the required information). For that purpose the following steps should do the trick:
    * backup all your customized handcrafted .nfo file (if you have any)
    * install nova version 6.xx
    * in nova settings unselect "process '.nfo' files"
    * in nova settings launch a "rescrape all" and wait for completion
    * in nova settings launch an "export already scraped videos" and wait for completion (**this step will override any existing .nfo file**)
* versions later than v6.0.30 targets API31 and due to Android storage restrictions for API30, local NFO/JPG media information files for videos stored on local storage have been moved to nova public application folder located /sdcard/Android/data/org.courville.nova/files/nfoPoster 
 * If you ever want to get back to nova v5.xx, you will need to clean application data *and cache*



[Changes][v6.0.67]


<a id="v6.0.66"></a>
## [v6.0.66 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.66) - 2022-05-15

- Add possibility to exclude network shortcuts from automatic/scheduled/manual global rescans on Android TV
- Optimize launch time on Android TV
- Stability enhancements

[Changes][v6.0.66]


<a id="v6.0.65"></a>
## [v6.0.65 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.65) - 2022-05-08

- Make animation row optional on android TV
- Add more blacklisted local storage directories to speed up media import
- Stability enhancements

[Changes][v6.0.65]


<a id="v6.0.64"></a>
## [v6.0.64 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.64) - 2022-05-03

- Stability enhancements
- New address for Sentry debug backend integration (crashlytics)

[Changes][v6.0.64]


<a id="v6.0.63"></a>
## [v6.0.63 amazon release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.63) - 2022-04-24

- Stability enhancements
- Fix adaptive refresh rate selection on firestick
- ffmpeg 4.4.2 and dav1d 1.0.0
- Fix fdroid build

[Changes][v6.0.63]


<a id="v6.0.62"></a>
## [v6.0.62 amazon release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.62) - 2022-04-18

Compared to previous release:
- Stability enhancements
- revert to ffmpeg 4.4.1 due to regression reported

[Changes][v6.0.62]


<a id="v5.15.21"></a>
## [v5.15.21 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.21) - 2021-09-01

- Fix crash on Android 12/S/API31
- Full screen display is enabled by default even on displays with cutouts
- Properly report DTS-HD and DTS-HD MA
- ffmpeg 4.4 and dav1d 0.9 integration 

[Changes][v5.15.21]


<a id="v5.15.20"></a>
## [v5.15.20 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.20) - 2021-05-09

- Better tv show subtitle download based on IMDB ID
- Disable delete on UPnP shares not supporting it



[Changes][v5.15.20]


<a id="v6.0.10"></a>
## [v6.0.10 beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.10) - 2021-03-26

- Add support for movie collections/sagas on Android TV
- Separate section for animation movies and series on Android TV
- Faster TV shows media information retrieval
- Fix scraping counter calculation on AndroidTV
- WARNING: media db upgrade to version 38 (any downgrade will wipe out your meta data)

**Important migration note:**

* This new version upgrades the internal nova media database to a new scheme and any downgrade to v4/v5 versions of nova will wipe out
 your entire video collection to prevent any incompatibility.
* Proper support for movie collections and animation movies/series on AndroidTV requires some manual steps. Acquisition of the additional movie collection informations and movies/TV series genres realignement requires a full rescrape of your video without interference of existing .nfo files (that do not yet contain the required information). For that purpose the following steps should do the trick:
    * backup all your customized handcrafted .nfo file (if you have any)
    * install nova version 6.x
    * in nova settings unselect "process '.nfo' files"
    * in nova settings launch a "rescrape all" and wait for completion
    * in nova settings launch an "export already scraped videos" and wait for completion (**this step will override any existing .nfo file**)

[Changes][v6.0.10]


<a id="v5.15.19"></a>
## [v5.15.19 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.19) - 2021-03-19

- Fix occasional SMB2/3 timeouts
- Add support for coloured TV remote buttons via HDMI-CEC
- ffmpeg version 4.3.2 and dav1d version 0.8.2 upstep



[Changes][v5.15.19]


<a id="v6.0.5"></a>
## [v6.0.5 movie collection experimental release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.5) - 2021-01-17

- Align with v5.16.17 with movie collections/sagas support on top


[Changes][v6.0.5]


<a id="v5.15.17"></a>
## [v5.15.17 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.17) - 2021-01-17

- SMBv2/3 support via jcifs-ng
- Use DNS,BCAST default SMB resolver order to avoid slow SMB share responses in some network configurations
- Allow AV1 hardware decoding
- Switch to NDK r22


[Changes][v5.15.17]


<a id="v4.49.16"></a>
## [v4.49.16 F-Droid only release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.16) - 2021-01-09

- Attempt to fix F-Droid server build
- dav1d update to 0.8.1


[Changes][v4.49.16]


<a id="v6.0.4"></a>
## [v6.0.4 movie collection experimental release](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.4) - 2021-01-07

- Align with v5.16.16 with movie collections/sagas support on top

[Changes][v6.0.4]


<a id="v5.15.16"></a>
## [v5.15.16 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.16) - 2021-01-07

- Align with v4.49.15 with latest jcifs-ng on top for SMBv2/3 support
- Fix non systematic wrong IP selected when browsing SMB shares
- New debug infrastructure based on slf4j/logback
- New 2021 banner icons for AndroidTV
- dav1d update to 0.8.1


[Changes][v5.15.16]


<a id="v5.15.15"></a>
## [v5.15.15 SMBv2/3 not so experimental release anymore](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.15) - 2020-12-08

- SMBv2/3 support via jcifs-ng
- Align with v4.49.15


[Changes][v5.15.15]


<a id="v4.49.15"></a>
## [v4.49.15 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.15) - 2020-12-08

- SMB1 support only rollback release aligned with v5.15.14 without jcifs-ng support to address SMB issue seen in the field
- Fix anime playback using opus track using libopus instead of platform one
- Update trakt/tmdb/thetvdb-java libraries to 6.8.5/2.2.0/2.4.0
- Restrict nova webview to nova usage
- Stability enhancements


[Changes][v4.49.15]


<a id="v5.15.14"></a>
## [v5.15.14 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.14) - 2020-12-06

- SMBv2/3 support via jcifs-ng
- Attempt to fix SMB on WD Mycloud with guest login


[Changes][v5.15.14]


<a id="v4.49.14"></a>
## [v4.49.14 rollback release for people with SMB issue](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.14) - 2020-12-06

Release for people having SMB connection issues with latest v5 releases.

[Changes][v4.49.14]


<a id="v6.0.3"></a>
## [v6.0.3 experimental release for movie collections](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.3) - 2020-12-03

- Align with v5.15.13 with movie collection/saga support



[Changes][v6.0.3]


<a id="v5.15.13"></a>
## [v5.15.13 Google Play release release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.13) - 2020-12-03

- Align with v4.49.11 with latest jcifs-ng on top
- Fix SMB timeout happening on some servers (jcifs-ng resolver)

[Changes][v5.15.13]


<a id="v6.0.1"></a>
## [v6.0.1 experimental release: support for movie collection](https://github.com/nova-video-player/aos-AVP/releases/tag/v6.0.1) - 2020-11-29

- Add support for movie collections/sagas for AndroidTV leanback interface

**Important note for migrating:** all already scraped movies do not contain any information about collections.
In order to add this missing information you need to rescrape the full movie collection.
A setting has been added to perform this task.
However, by default nova does process .nfo files which are exported part of the scraping which also does not contain movie collection information in order to speed up the scraping process.
These .nfo files when triggering a rescrape would be processed and would result into again no information found on collections.
Thus in order to get the movie collection data you need either to: deinstall/reinstall nova and delete all .nfo files on your internal storage or network shares or to follow these steps:
- install nova version 6.x
- in settings unselect "process '.nfo' files"
- in settings launch a "rescrape all movies" and wait for completion
- in settings launch an "export already scraped videos" and wait for completion

Current limitations:
- sometimes there is no poster/backdrop found for a collection: this is simply because TheMovieDb does not reference one



[Changes][v6.0.1]


<a id="v5.15.12"></a>
## [v5.15.12 github release with SMBv2/3 support](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.12) - 2020-12-03

- v4.49.12 with SMBv2/3 support via jcifs-ng on top


[Changes][v5.15.12]


<a id="v5.15.11"></a>
## [v5.15.11 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.11) - 2020-11-29

- SMBv2/3 support via jcifs-ng
- Fix anime playback using opus track using libopus instead of platform one
- Update trakt/tmdb/thetvdb-java libraries to 6.8.5/2.2.0/2.4.0
- Restrict nova webview to nova usage
- Stability enhancements


[Changes][v5.15.11]


<a id="v4.49.12"></a>
## [v4.49.12 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.12) - 2020-12-03

- Rollback to SMBv1 support only due to timeout issues with SMBv2 former release experienced by some users

[Changes][v4.49.12]


<a id="v5.15.10"></a>
## [v5.15.10 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.10) - 2020-10-23

- SMBv2/3 support via jcifs-ng
- Align with v4.49.11


[Changes][v5.15.10]


<a id="v4.49.11"></a>
## [v4.49.11 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.11) - 2020-10-23

- Stability enhancements


[Changes][v4.49.11]


<a id="v5.15.9"></a>
## [v5.15.9 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.9) - 2020-10-20

- SMBv2/3 support via jcifs-ng
- Align with v4.49.10

[Changes][v5.15.9]


<a id="v4.49.10"></a>
## [v4.49.10 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.10) - 2020-10-20

- Fix folder play mode
- Correct subtitles download failing while playing video on local storage


[Changes][v4.49.10]


<a id="v4.49.9"></a>
## [v4.49.9 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.9) - 2020-10-13

- Fix time displayed at video start on Android TV regression

[Changes][v4.49.9]


<a id="v5.15.7"></a>
## [v5.15.7 SMBv2/3 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.7) - 2020-10-11

- SMBv2/3 support via jcifs-ng
- Align with v4.49.8


[Changes][v5.15.7]


<a id="v4.49.8"></a>
## [v4.49.8 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.8) - 2020-10-11

- Do not stop local video playback on network connectivity change
- Use new nova icon for search bar
- Fix search crash on old Amazon firesticks
- Fix wrong player layout when screen rotation is locked and video started in portrait


[Changes][v4.49.8]


<a id="v5.15.6"></a>
## [v5.15.6 SMBv2/3 not so experimental release anymore](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.6) - 2020-09-25

- SMBv2/3 support via jcifs-ng
- Fix guest login on win10
- Align with v4.49.7


[Changes][v5.15.6]


<a id="v5.15.5"></a>
## [v5.15.5 SMBv2/3 not so experimental release anymore](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.5) - 2020-09-17

- Align with v4.49.7
- SMBv2/3 support via jcifs-ng


[Changes][v5.15.5]


<a id="v5.15.4"></a>
## [v5.15.4 SMBv2/3 not so experimental release anymore](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.4) - 2020-07-31

- Align with v4.49.6
- SMBv2/3 support via jcifs-ng


[Changes][v5.15.4]


<a id="v4.49.7"></a>
## [v4.49.7 Google play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.7) - 2020-09-17

- Display external storage label/description on AndroidTV
- Do not pollute subtitle manual picker with cached online retrieved subs
- Allow http video streaming
- chromeOS/Amazon UI fixes
- Add missing subtitles ISO639 code strings
- ffmpeg version 4.3.1 and dav1d version 0.7.1 upstep
- Stability enhancement


[Changes][v4.49.7]


<a id="v4.49.6"></a>
## [v4.49.6 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.6) - 2020-07-31

- Fix video stopping often on arm64 due to latest ffmpeg upstep
- Revert to ffmpeg 4.3.2 and dav1d 0.7.0


[Changes][v4.49.6]


<a id="v5.15.3"></a>
## [v5.15.3 SMBv2/3 not so experimental release anymore](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.3) - 2020-07-18

- Align with v4.49.5
- SMBv2/3 support via jcifs-ng
- fix SMB guest login on win10


[Changes][v5.15.3]


<a id="v5.15.2"></a>
## [v5.15.2 SMBv2/3 not so experimental release anymore](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.2) - 2020-07-11

- Align with v4.49.5 with latest jcifs-ng on top


[Changes][v5.15.2]


<a id="v4.49.5"></a>
## [v4.49.5 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.5) - 2020-07-11

- Fix x86 software decoding support (nexus player, non 64b chromebooks)
- Faster network scanning
- Stability enhancement

[Changes][v4.49.5]


<a id="v5.15.1"></a>
## [v5.15.1 SMBv2/3 experimental release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.15.1) - 2020-07-08

- Align with v4.49.3 with latest jcifs-ng on top
- Fix samba issues reported with WD MyCloud and with win10 guest login

[Changes][v5.15.1]


<a id="v4.49.3"></a>
## [v4.49.3 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.3) - 2020-07-07

- better USB disk management on AndroidTV
- Stability enhancement


[Changes][v4.49.3]


<a id="v4.49.2"></a>
## [v4.49.2 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.2) - 2020-07-06

- Fix OOM on Android TV with HDD plugged

[Changes][v4.49.2]


<a id="v4.49.1"></a>
## [v4.49.1 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.49.1) - 2020-07-04

- Fix number of audio tracks limited to 6
- ffmpeg version 4.3.0 and dav1d version 0.7.1 upstep
- Stability enhancement


[Changes][v4.49.1]


<a id="v4.48.17"></a>
## [v4.48.17 internal release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.17) - 2020-06-27

- Sponsor icon
- Reduce full compilation strain for boost


[Changes][v4.48.17]


<a id="v4.48.14"></a>
## [v4.48.14 internal release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.14) - 2020-06-23

- new release versioning management

[Changes][v4.48.14]


<a id="v4.48.13"></a>
## [v4.48.13 internal release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.13) - 2020-06-20

- new release versioning management

[Changes][v4.48.13]


<a id="v4.48.10"></a>
## [v4.48.10 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.10) - 2020-06-20

- Stability enhancement


[Changes][v4.48.10]


<a id="v4.48.9"></a>
## [v4.48.9 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.9) - 2020-06-12

- Fix missing poster on some movies
- Fix playback not smooth regression on Sony and Philips AndroidTV
- Stretch mode is back
- Allow adaptive refresh rate on phones
- Improve A/V sync for some videos (PTS instead of sample based sync)
- ffmpeg version 4.2.3 and dav1d version 0.7.0 upstep
- Scraping improvements
- Stability enhancement


[Changes][v4.48.9]


<a id="v4.48.8"></a>
## [v4.48.8 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.8) - 2020-05-30

- solve some A/V sync issues
- 0.7.0 dav1d and ffmpeg 4.2.3 upsteps
- faster boost compilation


[Changes][v4.48.8]


<a id="v4.48.7"></a>
## [v4.48.7 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.7) - 2020-05-18

- Intermediate release for fdroid
- fix java_home for linux


[Changes][v4.48.7]


<a id="v4.48.6"></a>
## [v4.48.6 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.6) - 2020-05-13

- Upgrade jsch for sftp support
- upgrade cling for UPnP support
- Stability enhancements


[Changes][v4.48.6]


<a id="v5.14.8"></a>
## [v5.14.8 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.14.8) - 2020-05-12

- Fix SMB server protocol level detection scheme
- Stability enhancements


[Changes][v5.14.8]


<a id="v4.48.5"></a>
## [v4.48.5 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.5) - 2020-05-13

- Upgrade jsch for sftp support


[Changes][v4.48.5]


<a id="v5.14.7"></a>
## [v5.14.7 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.14.7) - 2020-05-10

- Experimental SMBv2/3 support with latest jcifs-ng
- Support for SMBv2 is disabled by default and can be enabled in settings
- Disable SMB1/SMB2 protocol negotiation when SMB2 server is detected
- jsch update for sftp
- Stability enhancements


[Changes][v5.14.7]


<a id="v5.14.6"></a>
## [v5.14.6 intermediate release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.14.6) - 2020-05-09

- Disable SMB1/SMB2 protocol negotiation when SMB2 server is detected


[Changes][v5.14.6]


<a id="v4.48.4"></a>
## [v4.48.4 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.4) - 2020-05-10

Based on v4.48.3 with these changes:
- Stability enhancements


[Changes][v4.48.4]


<a id="v5.14.5"></a>
## [v5.14.5 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.14.5) - 2020-05-09

- Align with v4.48.3 with latest jcifs-ng on top for SMBv2/3 support
- Support for SMBv2 is disabled by default and can be enabled in settings

[Changes][v5.14.5]


<a id="v4.48.3"></a>
## [v4.48.3 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.3) - 2020-05-09

Based on v4.48.2 with these changes:
- Revert back jsch upstep since maven version without custom changes is too slow
- Stability enhancements


[Changes][v4.48.3]


<a id="v5.14.4"></a>
## [v5.14.4 SMBv2/3 experimental release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.14.4) - 2020-05-07

Align with v4.48.2 (unstable track) with following changes on top:
- Add SMBv2/3 support via jcifs-ng
- Support for SMBv2 is disabled by default and can be enabled in settings


[Changes][v5.14.4]


<a id="v4.48.2"></a>
## [v4.48.2 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.2) - 2020-05-03

Align with v4.48.0 (unstable track) with following changes on top:
- Fix ability to open videos via http/https from another application
- Improved scraping results
- UI navbar correct color on Samsung
- jsch update for sftp
- Stability enhancements


[Changes][v4.48.2]


<a id="v5.13.0"></a>
## [v5.13.0 SMBv2/3 experimental release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.13.0) - 2020-04-18

Align with v4.48 (unstable track) with following changes on top:
- Add SMBv2/3 support via jcifs-ng
- Fix slow video start on SMB by avoid checking .nomedia on server root

Note that this release might experience interoperability issues when using SMBv1 only capable server.



[Changes][v5.13.0]


<a id="v4.48.0"></a>
## [v4.48.0 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.48.0) - 2020-04-18

Align with v4.47 (unstable track) with following changes on top:
- Improve scraping results
- Stability enhancements


[Changes][v4.48.0]


<a id="v5.12"></a>
## [v5.12 SMBv2/3 experimental release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.12) - 2020-04-13

Align with v4.47 (unstable track) with following changes on top:
- Add SMBv2/3 support via jcifs-ng
- Fix samba file listing truncation when dealing with SMBv1 only servers
- Add opensubtitles credentials support in preferences since opensubtitles mandates it to download subtitles
- Fix an appcompat incompatibility with webview (Google bug)

Note that this release will experience interoperability issues when using SMBv1 only capable server.

[Changes][v5.12]


<a id="v4.47"></a>
## [v4.47 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.47) - 2020-04-12

Align with v4.46 (unstable track) with following changes on top:
- Fix trakt resume point sync issues


[Changes][v4.47]


<a id="v4.46"></a>
## [v4.46 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.46) - 2020-04-05

Align with v4.43 (unstable track) with following changes on top:
- Fix opensubtitles change requiring credentials to use API
- Fix DTSHD decoding crashes


[Changes][v4.46]


<a id="v4.44"></a>
## [v4.44 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.44) - 2020-04-05

Align with v4.38 (stable track) with following changes on top:
- Fix opensubtitles change requiring credentials to use API
- Fix DTSHD playback crashing sometimes


[Changes][v4.44]


<a id="v4.43"></a>
## [v4.43 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.43) - 2020-03-31

- Subtitle manual download improvement via scraped information search
- Better TV show scrape result through multi-language Levenshtein metric computation
- Refactored TmDb and TheTVDb scrapers
- UI polishing on phones/tablets and partners logo refresh (trakt, tmdb, tvdb, imdb)
- AppCompat migration


[Changes][v4.43]


<a id="v5.10"></a>
## [v5.10 SMBv2/3 experimental release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.10) - 2020-03-02

- Align with v4.40 with latest jcifs-ng on top

Note that this release will experience interoperability issues when using SMBv1 only capable server.


[Changes][v5.10]


<a id="v4.40"></a>
## [v4.40 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.40) - 2020-03-02

- Refactored TmDb and TheTVDb scrapers
- Better TV show scrape result through multi-language Levenshtein metric computation
- Fix crash observed on play console
- Use new application icon for TV channels


[Changes][v4.40]


<a id="v4.39"></a>
## [v4.39 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.39) - 2020-03-02

- Fix crash observed on play console
- Use new application icon for TV channels


[Changes][v4.39]


<a id="v5.9"></a>
## [v5.9 SMBv2/3 experimental release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.9) - 2020-03-01

- Align with 4.38 with latest jcifs-ng on top


[Changes][v5.9]


<a id="v4.38"></a>
## [v4.38 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.38) - 2020-02-29

- Better show scraper with multi-lang Levenshtein metric computation
- Fix cloud storage (file picker) and folder picker on phones


[Changes][v4.38]


<a id="v4.37"></a>
## [v4.37 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.37) - 2020-02-29

- Fix cloud storage (file picker) and folder picker on phones


[Changes][v4.37]


<a id="v4.36"></a>
## [v4.36 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.36) - 2020-02-22

- Roll back to old MovieScraper2
- 10ms audio/video delay tuning
- Latest translations


[Changes][v4.36]


<a id="v4.35"></a>
## [v4.35 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.35) - 2020-02-08

- Switch to Audiotrack audio interface for video fluidity
- Fix TV show Trakt progress sync
- tmdb-java movie scraper
- Adaptive refresh rate via API23 mode switch (fix FireTV4k)
- Fix grey bar on Sony for HDR content
- Fix green bar with swdec on Nvidia
- Fix audio night/boost mode
- Fix HEVC 10b on Rockchip
- Better MediaCodec extradata management
- Turkish/Simplified Chinese translations completed
- New app icon
- App bundles to reduce apk size
- Limit SMB discovery on local networks


[Changes][v4.35]


<a id="v4.28.3"></a>
## [v4.28.3 release (stable track)](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.28.3) - 2020-02-08

- Fix TV show Trakt progress sync
- Fix grey bar issue on Sony when watching HDR content
- Fix green bars present in software decoding on Nvidia shield
- Fix audio regressions in night/boost mode
- Fix video not opening when enabling adaptive refresh rate on FireTV

[Changes][v4.28.3]


<a id="v5.8"></a>
## [v5.8 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.8) - 2020-01-24

- Align with v4.33 with jcifs-ng on top


[Changes][v5.8]


<a id="v4.33"></a>
## [v4.33 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.33) - 2020-01-24

- Fix regression in TV show not recognized due to TheTVdb backend unilateral change

[Changes][v4.33]


<a id="v4.30"></a>
## [v4.30 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.30) - 2020-01-22

- Use Audiotrack vs. OpenSLES for audio interface improving video fluidity
- Fix TV show Trakt progress sync
- Disable periodic bookmark save interfering with video decoding perf over slow network shares
- Complete Turkish & Simplified Chinese translations
- New icon compliant with Google Play Store requirements
- Only launch SMB discovery on local networks


[Changes][v4.30]


<a id="v4.29"></a>
## [v4.29 Google play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.29) - 2020-01-11

- Fix HEVC 10 bit support on Rockchip devices
- Better extradata management for AVC and HEVC for MediaCodec
- Stability enhancements


[Changes][v4.29]


<a id="v4.28"></a>
## [v4.28 Google play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.28) - 2020-01-11

- Prefer ffmpeg over c2.android or omx.google software codecs to avoid multimedia issues on pixel3xl phone
- Stability enhancements


[Changes][v4.28]


<a id="v4.27"></a>
## [v4.27 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.27) - 2020-01-05

- ffmpeg update to 4.2.2
- dav1d update to 0.5.2
- Break video import and scrape in small queries to avoid database window cursor issues
- Stability enhancement


[Changes][v4.27]


<a id="v4.26"></a>
## [v4.26 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.26) - 2019-12-29

- Better scrape result through Levenshtein result distance computation
- Stability enhancement


[Changes][v4.26]


<a id="v4.25"></a>
## [v4.25 release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.25) - 2019-12-26

- Introduce stretched video format to fill entire display with video image (only way to preserve aspect ratio on recent Philips TVs!)
- Add Norwegian, Vietnamese scrape languages support
- 2020 year banners for Android TV
- Improve filename pre-processing garbage rules to improve scrape
- Prevent scrape notification to fire up when nothing is to be scraped
- Fix sftp indexing


[Changes][v4.25]


<a id="v5.7"></a>
## [v5.7 SMBv2 beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.7) - 2019-12-14

- Align with v4.24 with jcifs-ng on top

[Changes][v5.7]


<a id="v4.24"></a>
## [v4.24 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.24) - 2019-12-14

- Fix more shows not being scraped correctly after thetvdb.com site changes
- Rollback on jcsh upgrade yielding issues on sftp
- Fix regression in pause/play with enter key on AndroidTV
- Fix some aspect ratio issues on devices where MediaCodec returns wrong video dimensions (firetv4k, rockchip, etc.)
- Reduce bottom player UI glitch on chromebook and rockchip leanback interfaces

[Changes][v4.24]


<a id="v4.22"></a>
## [v4.22 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.22) - 2019-12-08

- Fix some shows not being scraped correctly after thetvdb.com site changes
- Fix player controller UI layout issues on tablets
- Update thetvdb-java to version 2.2.0

[Changes][v4.22]


<a id="v4.21"></a>
## [v4.21 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.21) - 2019-12-08

- Faster AndroidTV display entering application
- Attempt to fix an UI glitch on Rockchip based TV boxes
- Stability enhancements

[Changes][v4.21]


<a id="v5.6"></a>
## [v5.6 SMBv2 beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.6) - 2019-12-01

Unstable branch: this release is based on minSDK 21, targetSDK 29, AndroidX libraries, NDK-r20, ffmpeg 4.2.1.
- Fix SMBv1 guest/anonymous auth on freebox

[Changes][v5.6]


<a id="v4.20"></a>
## [v4.20 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.20) - 2019-12-01

Testing branch: this release is based on minSDK 21, targetSDK 29, AndroidX libraries, NDK-r20, ffmpeg 4.2.1.
- Stability enhancements

[Changes][v4.20]


<a id="v4.18"></a>
## [v4.18 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.18) - 2019-11-22

Testing branch: this release is based on minSDK 21, targetSDK 29, AndroidX libraries, NDK-r20, ffmpeg 4.2.1.
- Fix player crashing in Dutch due to translation error
- Fix TV shows meta data retrieval issues due to to TheTVdb.com backend changes


[Changes][v4.18]


<a id="v4.16"></a>
## [v4.16 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.16) - 2019-11-16

Testing branch: this release is based on minSDK 21, targetSDK 29, AndroidX libraries, NDK-r20, ffmpeg 4.2.1.
- Migration to TheTVDB API v2 via thetvdb-java external library with request caching support
- Target API29 disabling scoped storage for now
- Indexing, scraping and file copy proper foreground notifications
- Stability enhancements

Remark: this version only supports SMBv1 (rollback due to problems reported with jcifs-ng switch)

[Changes][v4.16]


<a id="v5.3"></a>
## [v5.3 Google play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.3) - 2019-11-03

Testing branch: this release is based on minSDK 21, targetSDK 29, AndroidX libraries, NDK-r20, ffmpeg 4.2.1.
- Leanback setting style for subtitles languages download
- Remove systematic video background reload in VideoDetailsFragment on leadback when back from video play
- Stability enhancements

[Changes][v5.3]


<a id="v5.2"></a>
## [v5.2 Google play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.2) - 2019-10-27

Testing branch: this release is based on minSDK 21, targetSDK 29, AndroidX libraries, NDK-r20, ffmpeg 4.2.1.
- Fix selection of torrent streaming download directory not selectable
- Indexing, scraping and file copy proper foreground notifications
- Stability enhancements

[Changes][v5.2]


<a id="v5.1"></a>
## [v5.1 unstable release](https://github.com/nova-video-player/aos-AVP/releases/tag/v5.1) - 2019-09-21

Unstable branch: this release is based on minSDK 21, targetSDK 29, AndroidX libraries, NDK-r20, ffmpeg 4.2.1.
- Switch to jcifs-ng to support SMBv2/3
- Target API29 (Android Q) and disable scoped storage for now
- Fix crash entering settings on phones with cutout

[Changes][v5.1]


<a id="v4.15"></a>
## [v4.15 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.15) - 2019-09-21

Testing branch: this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.1.
- Fix resume point update on VideoInfoActivity and auto scraping of unknown files on network shares


[Changes][v4.15]


<a id="v4.14"></a>
## [v4.14 Google play beta release candidate](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.14) - 2019-09-15

"Not so much anymore unstable branch": this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.1.
- Only switch to AudioTrack instead of openSLES to solve audio/video delay on Amlogic
- Upgrade to latest version of trakt-java containing NVP upstreamed contribution
- Add support for codepade 28606 - Latin-10 or South-Eastern European for subs

[Changes][v4.14]


<a id="v4.13"></a>
## [v4.13 Google play beta release candidate](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.13) - 2019-09-08

"Not so much anymore unstable branch": this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.
- Switch to AudioTrack instead of openSLES to solve audio/video delay on some devices
- Disable for now UpNext row/channel preventing display of indexed folders
- Upgrade trakt-java library to solve two way sync

[Changes][v4.13]


<a id="v4.12"></a>
## [v4.12 Google play beta release candidate](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.12) - 2019-08-29

"Not so much anymore unstable branch": this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.
- Fix HEVC decoding for some files on MTK based devices
- Do not revert on SW decoding in presence of high bitrate spike occurring on some 4k high bitrate videos

[Changes][v4.12]


<a id="v4.11"></a>
## [v4.11 Google play beta release candidate](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.11) - 2019-08-28

"Not so much anymore unstable branch": this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.
- Fix coexistence with Archos Video Player

[Changes][v4.11]


<a id="v4.10"></a>
## [v4.10 Google play beta release candidate](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.10) - 2019-08-22

"Not so much anymore unstable branch": this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.
- Fix video blacklisting on local storage

[Changes][v4.10]


<a id="v4.9"></a>
## [v4.9 Google play beta release candidate](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.9) - 2019-08-21

"Not so much anymore unstable branch": this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.
- FFmpeg upstep to 4.2 and dav1d to 0.4.0
- Fix database crash preventing application to start on some custom ROMs

[Changes][v4.9]


<a id="v4.8"></a>
## [v4.8 unstable release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.8) - 2019-08-02

Unstable branch: this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.
- Fix database crash preventing application to start on some devices

[Changes][v4.8]


<a id="v3.12"></a>
## [v3.12 Google play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v3.12) - 2019-08-02

Testing branch: this release is based on minSDK 21, targetSDK 27, NDK-r20, ffmpeg 4.2.
- Fix database crash preventing application to start on some devices



[Changes][v3.12]


<a id="v4.7"></a>
## [v4.7 unstable release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.7) - 2019-06-15

Unstable branch: this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.
- Improve audio passthrough robustness
- Fix authentication issue with Trakt

[Changes][v4.7]


<a id="v3.11"></a>
## [v3.11 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v3.11) - 2019-06-15

Testing branch: this release is based on minSDK 21, targetSDK 27, NDK-r20, ffmpeg 4.2.
- Improve audio passthrough robustness

[Changes][v3.11]


<a id="v3.10"></a>
## [v3.10 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v3.10) - 2019-06-09

- Fix authentication issue with Trakt

[Changes][v3.10]


<a id="v4.6"></a>
## [v4.6 unstable release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.6) - 2019-06-03

Unstable branch: this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r19c, ffmpeg 4.2.
- Attempt to fix UPnP playback of files containing a "/"
- Do not crash when opening non-video files in browser
- Stability improvements

[Changes][v4.6]


<a id="v3.9"></a>
## [v3.9 Google play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v3.9) - 2019-06-03

Testing branch: this release is based on minSDK 21, targetSDK 27, NDK-r19c, ffmpeg 4.2.
- Attempt to fix UPnP playback of files containing a "/"
- Do not crash when opening non-video files in browser
- Stability improvements

[Changes][v3.9]


<a id="v4.5"></a>
## [v4.5 unstable release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.5) - 2019-05-30

Unstable branch: this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.
- Fix files cannot play from external sdcard using an external player
- AndroidTV: fix EpisodesByDate week view crash in case of large TV show collection

[Changes][v4.5]


<a id="v3.8"></a>
## [v3.8 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v3.8) - 2019-05-30

Testing branch: this release is based on minSDK 21, targetSDK 27, NDK-r20, ffmpeg 4.2.
- Fix files cannot play from external sdcard using an external player

[Changes][v3.8]


<a id="v4.3"></a>
## [v4.3 unstable release](https://github.com/nova-video-player/aos-AVP/releases/tag/v4.3) - 2019-05-19

Unstable branch: this release is based on minSDK 21, targetSDK 28, AndroidX libraries, NDK-r20, ffmpeg 4.2.
- Scanning and scraping proper Notifications
- Add an option to force disabling stereo downmix on phones/tablets with Android version > N
- AndroidTV: add pinning on long press for all movies/tvshows
- New TV show categories for quicker browsing through large collection
- Countless TV UI improvements (roles, trailers, badges, global del/deindex, subs picker)
- New player shortcuts (A/S switch audio/sub track, U/D = volume up/down) and menu support
- Improve audio passthrough stability
- Fix sftp playback interruptions
- Make private mode persistent
- Fix cloud support (still no streaming)- AndroidTV: add poster/backdrop zoom on long press
- AndroidTV: add tvshow episodes by date view
- Fix sftp playback interruptions
- Fix an android Q DP3 crash

[Changes][v4.3]


<a id="v3.7"></a>
## [v3.7 Google Play release](https://github.com/nova-video-player/aos-AVP/releases/tag/v3.7) - 2019-05-19

Testing branch: this release is based on minSDK 21, targetSDK 27, NDK-r20, ffmpeg 4.2.
- Re-enable downmix on phones to avoid voice channels loss on some phones
- Stability improvements
- Upgrade to latest ffmpeg and dav1d soft codecs

[Changes][v3.7]


<a id="v2.2"></a>
## [v2.2 Google Play release candidate](https://github.com/nova-video-player/aos-AVP/releases/tag/v2.2) - 2019-05-19

Stable branch: this release is based on minSDK 17, targetSDK 27, NDK-r16b, ffmpeg 3.3.x.
- New TV show categories for quicker browsing through large collection
- Countless TV UI improvements (roles, trailers, badges, global del/deindex, subs picker)
- New player shortcuts (A/S switch audio/sub track, U/D = volume up/down) and menu support
- Improve audio passthrough stability
- Fix sftp playback interruptions
- Make private mode persistent
- Fix cloud support (still no streaming)

[Changes][v2.2]


<a id="v3.1"></a>
## [v3.1 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v3.1) - 2019-02-03

Testing branch: this release is based on minSDK 21, targetSDK 27, NDK-r19, ffmpeg 4.2.
- New TV show categories on TV interface for quicker browsing through large collection

[Changes][v3.1]


<a id="v3.0"></a>
## [v3.0 Google Play beta release](https://github.com/nova-video-player/aos-AVP/releases/tag/v3.0) - 2019-01-30

Testing branch: this release is based on minSDK 21, targetSDK 27, NDK-r19, ffmpeg 4.2.
- Migration from Android ndk-r17 to ndk-r19
- Add AV1 soft decoding capability through 4.2-dev ffmpeg version and dav1d codec
- Add support for x86_64 architecture
- Improve audio passthrough stability
- Make private mode persistent between application relaunches

[Changes][v3.0]


<a id="v2.1"></a>
## [v2.1 Google Play public release](https://github.com/nova-video-player/aos-AVP/releases/tag/v2.1) - 2018-09-20

Stable branch: this release is based on minSDK 17, targetSDK 27, NDK-r16b, ffmpeg 3.3.x.
- Improved french translations and interfacing with crowdin service
- Stability improvements

[Changes][v2.1]


<a id="v2.0"></a>
## [v2.0 Google Play public release](https://github.com/nova-video-player/aos-AVP/releases/tag/v2.0) - 2018-09-07

Stable branch: this release is based on minSDK 17, targetSDK 27, NDK-r16b, ffmpeg 3.3.x.
- Scraper improvements and bug fixes
- Issue a warning toast is hardware decoding is disabled

[Changes][v2.0]


<a id="v1.0"></a>
## [v1.0 Initial Google Play public release](https://github.com/nova-video-player/aos-AVP/releases/tag/v1.0) - 2018-08-26

Stable branch: this release is based on minSDK 17, targetSDK 27, NDK-r16b, ffmpeg 3.3.x.
- Add support for Android P avoiding application crash at startup
- Add a "list episodes" button on tvshow episode view to quickly get to tvshow view on AndroidTV leanback version
- Add notification channels for Oreo
- Fix subtitle delay not applied on play resume when negative
- Fix floating player crash on Android version Oreo and above
- Fix loss of activity background and private mode background
- Prevent from playing a file when detecting a problem: issue a toast instead

[Changes][v1.0]


[v6.3.27]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.26...v6.3.27
[v6.3.26]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.25...v6.3.26
[v6.3.25]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.24...v6.3.25
[v6.3.24]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.23...v6.3.24
[v6.3.23]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.22...v6.3.23
[v6.3.22]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.21...v6.3.22
[v6.3.21]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.20...v6.3.21
[v6.3.20]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.19...v6.3.20
[v6.3.19]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.18...v6.3.19
[v6.3.18]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.17...v6.3.18
[v6.3.17]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.16...v6.3.17
[v6.3.16]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.15...v6.3.16
[v6.3.15]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.14...v6.3.15
[v6.3.14]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.13...v6.3.14
[v6.3.13]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.12...v6.3.13
[v6.3.12]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.11...v6.3.12
[v6.3.11]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.10...v6.3.11
[v6.3.10]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.6...v6.3.10
[v6.3.6]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.5...v6.3.6
[v6.3.5]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.4...v6.3.5
[v6.3.4]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.3...v6.3.4
[v6.3.3]: https://github.com/nova-video-player/aos-AVP/compare/v6.3.2...v6.3.3
[v6.3.2]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.95...v6.3.2
[v6.2.95]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.93...v6.2.95
[v6.2.93]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.92...v6.2.93
[v6.2.92]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.91...v6.2.92
[v6.2.91]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.90...v6.2.91
[v6.2.90]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.89...v6.2.90
[v6.2.89]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.88...v6.2.89
[v6.2.88]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.87...v6.2.88
[v6.2.87]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.86...v6.2.87
[v6.2.86]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.85...v6.2.86
[v6.2.85]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.84...v6.2.85
[v6.2.84]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.82...v6.2.84
[v6.2.82]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.81...v6.2.82
[v6.2.81]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.79...v6.2.81
[v6.2.79]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.78...v6.2.79
[v6.2.78]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.77...v6.2.78
[v6.2.77]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.76...v6.2.77
[v6.2.76]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.75...v6.2.76
[v6.2.75]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.74...v6.2.75
[v6.2.74]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.73...v6.2.74
[v6.2.73]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.72...v6.2.73
[v6.2.72]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.71...v6.2.72
[v6.2.71]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.70...v6.2.71
[v6.2.70]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.69...v6.2.70
[v6.2.69]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.67...v6.2.69
[v6.2.67]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.66...v6.2.67
[v6.2.66]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.65...v6.2.66
[v6.2.65]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.64...v6.2.65
[v6.2.64]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.63...v6.2.64
[v6.2.63]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.62...v6.2.63
[v6.2.62]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.61...v6.2.62
[v6.2.61]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.59...v6.2.61
[v6.2.59]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.58...v6.2.59
[v6.2.58]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.57...v6.2.58
[v6.2.57]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.55...v6.2.57
[v6.2.55]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.54...v6.2.55
[v6.2.54]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.53...v6.2.54
[v6.2.53]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.52...v6.2.53
[v6.2.52]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.51...v6.2.52
[v6.2.51]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.50...v6.2.51
[v6.2.50]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.49...v6.2.50
[v6.2.49]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.48...v6.2.49
[v6.2.48]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.47...v6.2.48
[v6.2.47]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.46...v6.2.47
[v6.2.46]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.44...v6.2.46
[v6.2.44]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.43...v6.2.44
[v6.2.43]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.40...v6.2.43
[v6.2.40]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.38...v6.2.40
[v6.2.38]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.37...v6.2.38
[v6.2.37]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.36...v6.2.37
[v6.2.36]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.35...v6.2.36
[v6.2.35]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.34...v6.2.35
[v6.2.34]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.33...v6.2.34
[v6.2.33]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.32...v6.2.33
[v6.2.32]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.31...v6.2.32
[v6.2.31]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.30...v6.2.31
[v6.2.30]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.29...v6.2.30
[v6.2.29]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.28...v6.2.29
[v6.2.28]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.17...v6.2.28
[v6.2.17]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.16...v6.2.17
[v6.2.16]: https://github.com/nova-video-player/aos-AVP/compare/v6.2.15...v6.2.16
[v6.2.15]: https://github.com/nova-video-player/aos-AVP/compare/v6.1.6...v6.2.15
[v6.1.6]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.97...v6.1.6
[v6.0.97]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.96...v6.0.97
[v6.0.96]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.95...v6.0.96
[v6.0.95]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.94...v6.0.95
[v6.0.94]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.93...v6.0.94
[v6.0.93]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.89...v6.0.93
[v6.0.89]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.88...v6.0.89
[v6.0.88]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.87...v6.0.88
[v6.0.87]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.83...v6.0.87
[v6.0.83]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.82...v6.0.83
[v6.0.82]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.81...v6.0.82
[v6.0.81]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.80...v6.0.81
[v6.0.80]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.79...v6.0.80
[v6.0.79]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.76...v6.0.79
[v6.0.76]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.75...v6.0.76
[v6.0.75]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.71...v6.0.75
[v6.0.71]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.70...v6.0.71
[v6.0.70]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.67...v6.0.70
[v6.0.67]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.66...v6.0.67
[v6.0.66]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.65...v6.0.66
[v6.0.65]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.64...v6.0.65
[v6.0.64]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.63...v6.0.64
[v6.0.63]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.62...v6.0.63
[v6.0.62]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.21...v6.0.62
[v5.15.21]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.20...v5.15.21
[v5.15.20]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.10...v5.15.20
[v6.0.10]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.19...v6.0.10
[v5.15.19]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.5...v5.15.19
[v6.0.5]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.17...v6.0.5
[v5.15.17]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.16...v5.15.17
[v4.49.16]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.4...v4.49.16
[v6.0.4]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.16...v6.0.4
[v5.15.16]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.15...v5.15.16
[v5.15.15]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.15...v5.15.15
[v4.49.15]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.14...v4.49.15
[v5.15.14]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.14...v5.15.14
[v4.49.14]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.3...v4.49.14
[v6.0.3]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.13...v6.0.3
[v5.15.13]: https://github.com/nova-video-player/aos-AVP/compare/v6.0.1...v5.15.13
[v6.0.1]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.12...v6.0.1
[v5.15.12]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.11...v5.15.12
[v5.15.11]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.12...v5.15.11
[v4.49.12]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.10...v4.49.12
[v5.15.10]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.11...v5.15.10
[v4.49.11]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.9...v4.49.11
[v5.15.9]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.10...v5.15.9
[v4.49.10]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.9...v4.49.10
[v4.49.9]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.7...v4.49.9
[v5.15.7]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.8...v5.15.7
[v4.49.8]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.6...v4.49.8
[v5.15.6]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.5...v5.15.6
[v5.15.5]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.4...v5.15.5
[v5.15.4]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.7...v5.15.4
[v4.49.7]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.6...v4.49.7
[v4.49.6]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.3...v4.49.6
[v5.15.3]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.2...v5.15.3
[v5.15.2]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.5...v5.15.2
[v4.49.5]: https://github.com/nova-video-player/aos-AVP/compare/v5.15.1...v4.49.5
[v5.15.1]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.3...v5.15.1
[v4.49.3]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.2...v4.49.3
[v4.49.2]: https://github.com/nova-video-player/aos-AVP/compare/v4.49.1...v4.49.2
[v4.49.1]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.17...v4.49.1
[v4.48.17]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.14...v4.48.17
[v4.48.14]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.13...v4.48.14
[v4.48.13]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.10...v4.48.13
[v4.48.10]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.9...v4.48.10
[v4.48.9]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.8...v4.48.9
[v4.48.8]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.7...v4.48.8
[v4.48.7]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.6...v4.48.7
[v4.48.6]: https://github.com/nova-video-player/aos-AVP/compare/v5.14.8...v4.48.6
[v5.14.8]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.5...v5.14.8
[v4.48.5]: https://github.com/nova-video-player/aos-AVP/compare/v5.14.7...v4.48.5
[v5.14.7]: https://github.com/nova-video-player/aos-AVP/compare/v5.14.6...v5.14.7
[v5.14.6]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.4...v5.14.6
[v4.48.4]: https://github.com/nova-video-player/aos-AVP/compare/v5.14.5...v4.48.4
[v5.14.5]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.3...v5.14.5
[v4.48.3]: https://github.com/nova-video-player/aos-AVP/compare/v5.14.4...v4.48.3
[v5.14.4]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.2...v5.14.4
[v4.48.2]: https://github.com/nova-video-player/aos-AVP/compare/v5.13.0...v4.48.2
[v5.13.0]: https://github.com/nova-video-player/aos-AVP/compare/v4.48.0...v5.13.0
[v4.48.0]: https://github.com/nova-video-player/aos-AVP/compare/v5.12...v4.48.0
[v5.12]: https://github.com/nova-video-player/aos-AVP/compare/v4.47...v5.12
[v4.47]: https://github.com/nova-video-player/aos-AVP/compare/v4.46...v4.47
[v4.46]: https://github.com/nova-video-player/aos-AVP/compare/v4.44...v4.46
[v4.44]: https://github.com/nova-video-player/aos-AVP/compare/v4.43...v4.44
[v4.43]: https://github.com/nova-video-player/aos-AVP/compare/v5.10...v4.43
[v5.10]: https://github.com/nova-video-player/aos-AVP/compare/v4.40...v5.10
[v4.40]: https://github.com/nova-video-player/aos-AVP/compare/v4.39...v4.40
[v4.39]: https://github.com/nova-video-player/aos-AVP/compare/v5.9...v4.39
[v5.9]: https://github.com/nova-video-player/aos-AVP/compare/v4.38...v5.9
[v4.38]: https://github.com/nova-video-player/aos-AVP/compare/v4.37...v4.38
[v4.37]: https://github.com/nova-video-player/aos-AVP/compare/v4.36...v4.37
[v4.36]: https://github.com/nova-video-player/aos-AVP/compare/v4.35...v4.36
[v4.35]: https://github.com/nova-video-player/aos-AVP/compare/v4.28.3...v4.35
[v4.28.3]: https://github.com/nova-video-player/aos-AVP/compare/v5.8...v4.28.3
[v5.8]: https://github.com/nova-video-player/aos-AVP/compare/v4.33...v5.8
[v4.33]: https://github.com/nova-video-player/aos-AVP/compare/v4.30...v4.33
[v4.30]: https://github.com/nova-video-player/aos-AVP/compare/v4.29...v4.30
[v4.29]: https://github.com/nova-video-player/aos-AVP/compare/v4.28...v4.29
[v4.28]: https://github.com/nova-video-player/aos-AVP/compare/v4.27...v4.28
[v4.27]: https://github.com/nova-video-player/aos-AVP/compare/v4.26...v4.27
[v4.26]: https://github.com/nova-video-player/aos-AVP/compare/v4.25...v4.26
[v4.25]: https://github.com/nova-video-player/aos-AVP/compare/v5.7...v4.25
[v5.7]: https://github.com/nova-video-player/aos-AVP/compare/v4.24...v5.7
[v4.24]: https://github.com/nova-video-player/aos-AVP/compare/v4.22...v4.24
[v4.22]: https://github.com/nova-video-player/aos-AVP/compare/v4.21...v4.22
[v4.21]: https://github.com/nova-video-player/aos-AVP/compare/v5.6...v4.21
[v5.6]: https://github.com/nova-video-player/aos-AVP/compare/v4.20...v5.6
[v4.20]: https://github.com/nova-video-player/aos-AVP/compare/v4.18...v4.20
[v4.18]: https://github.com/nova-video-player/aos-AVP/compare/v4.16...v4.18
[v4.16]: https://github.com/nova-video-player/aos-AVP/compare/v5.3...v4.16
[v5.3]: https://github.com/nova-video-player/aos-AVP/compare/v5.2...v5.3
[v5.2]: https://github.com/nova-video-player/aos-AVP/compare/v5.1...v5.2
[v5.1]: https://github.com/nova-video-player/aos-AVP/compare/v4.15...v5.1
[v4.15]: https://github.com/nova-video-player/aos-AVP/compare/v4.14...v4.15
[v4.14]: https://github.com/nova-video-player/aos-AVP/compare/v4.13...v4.14
[v4.13]: https://github.com/nova-video-player/aos-AVP/compare/v4.12...v4.13
[v4.12]: https://github.com/nova-video-player/aos-AVP/compare/v4.11...v4.12
[v4.11]: https://github.com/nova-video-player/aos-AVP/compare/v4.10...v4.11
[v4.10]: https://github.com/nova-video-player/aos-AVP/compare/v4.9...v4.10
[v4.9]: https://github.com/nova-video-player/aos-AVP/compare/v4.8...v4.9
[v4.8]: https://github.com/nova-video-player/aos-AVP/compare/v3.12...v4.8
[v3.12]: https://github.com/nova-video-player/aos-AVP/compare/v4.7...v3.12
[v4.7]: https://github.com/nova-video-player/aos-AVP/compare/v3.11...v4.7
[v3.11]: https://github.com/nova-video-player/aos-AVP/compare/v3.10...v3.11
[v3.10]: https://github.com/nova-video-player/aos-AVP/compare/v4.6...v3.10
[v4.6]: https://github.com/nova-video-player/aos-AVP/compare/v3.9...v4.6
[v3.9]: https://github.com/nova-video-player/aos-AVP/compare/v4.5...v3.9
[v4.5]: https://github.com/nova-video-player/aos-AVP/compare/v3.8...v4.5
[v3.8]: https://github.com/nova-video-player/aos-AVP/compare/v4.3...v3.8
[v4.3]: https://github.com/nova-video-player/aos-AVP/compare/v3.7...v4.3
[v3.7]: https://github.com/nova-video-player/aos-AVP/compare/v2.2...v3.7
[v2.2]: https://github.com/nova-video-player/aos-AVP/compare/v3.1...v2.2
[v3.1]: https://github.com/nova-video-player/aos-AVP/compare/v3.0...v3.1
[v3.0]: https://github.com/nova-video-player/aos-AVP/compare/v2.1...v3.0
[v2.1]: https://github.com/nova-video-player/aos-AVP/compare/v2.0...v2.1
[v2.0]: https://github.com/nova-video-player/aos-AVP/compare/v1.0...v2.0
[v1.0]: https://github.com/nova-video-player/aos-AVP/tree/v1.0

<!-- Generated by https://github.com/rhysd/changelog-from-release v3.8.1 -->

