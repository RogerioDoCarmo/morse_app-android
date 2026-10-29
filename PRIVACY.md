# Privacy Policy — OmniMorse (F-Droid build)

Last updated: 28 October 2026.

The OmniMorse build published on F-Droid is built from this same source with
crash reporting and update checks removed. For that build, this section is the
whole policy.

## What stays on your device

**Your settings.** The dot/dash cut-off, playback speed, interface language,
speech-recognition language, and whether decoded text is read aloud. Also a note
of whether you have seen the welcome guide. They are stored in the app's own
storage and deleted when you uninstall the app.

**Your messages.** Anything you type, tap in, or speak is translated on your
device and held only while the app is open. Nothing you write is stored between
sessions.

## What can leave your device

**Nothing the app sends itself.** It has no internet permission, so it cannot
open a network connection. There are no crash reports, no analytics and no
update checks.

**Speech input is the one exception.** On the Speak tab the app asks your
device's own speech-recognition service to turn what you say into text.
Depending on which service is installed, it may send your audio to its provider
to be transcribed; on most phones that service is Google's. OmniMorse receives
only the resulting text, holds it in memory, and discards it when you leave the
screen. This is why F-Droid lists the app with the NonFreeNet anti-feature.

Reading decoded text aloud uses your device's own text-to-speech engine.

## What the app asks permission for, and why

**Camera**: used only to switch the torch on and off, so a message can be
played as light. The camera preview is never opened and no image is ever
captured.

**Microphone**: used only while you are on the Speak tab with recording
active, to turn speech into text as described above.

Both permissions are optional. Everything else in the app works without them.

## Contact

Questions about this policy: <contact@rogeriodocarmo.com>

Source code: <https://github.com/RogerioDoCarmo/morse_app>
