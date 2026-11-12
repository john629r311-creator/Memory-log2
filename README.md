# Memory Recall Keyboard — local activity and key-count journal

Android Java project. The keyboard **does not store characters or passwords**. It counts character insertions, spaces, backspaces, and Enter actions during ordinary typing sessions. Password-type input fields are excluded from session storage. These are key actions handled by this keyboard, not a guarantee of changes in the text field (e.g. autocorrect, paste, hardware keyboard).

The keyboard displays a recording indicator. The main app requires consent and allows withdrawal, permission setup, and manual report saving. Android Usage Access is required for app usage events.

Reports are written to app-specific Documents/MemoryRecallLogs, with names such as `log-11-12-26-1030am.txt`. Android may delay periodic background jobs; files may be difficult to access in some file managers and may be removed when uninstalling.

## Build

Open this folder as a Gradle Android project in a compatible Android IDE. Use JDK 17, Android SDK platform 35 and Android Gradle Plugin 8.6.1 (Gradle 8.7). Build the `app` debug variant. The project has not been compiled in this environment; the Android SDK and Gradle are not installed here.

## Usage

Open the app, accept the consent screen, grant Usage Access, enable the Memory Recall keyboard in Android input-method settings, and select it. Reports can be saved manually; periodic jobs are best effort.


Blue-dot update: small blue status dot at top right of keyboard while non-sensitive key counts are tracked. Gray dot for password fields. Tap the dot for a plain-language explanation. No raw text or passwords are saved.
