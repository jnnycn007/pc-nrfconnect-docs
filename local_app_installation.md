---
---

# Installing local apps

When you start nRF Connect for Desktop, it shows a list of
all apps officially supported by Nordic Semiconductors. But if you create
new apps or new versions, you can also
[create a developer bundle of an app](./app_development#distributing-development-versions)
consisting of a file like `pc-nrfconnect-boilerplate-0.0.1.tgz`, which users
can install manually.

The easiest way to install a local app is by dropping the bundle file onto the
apps list of the nRF Connect for Desktop window. This also requires no restart
of nRF Connect for Desktop.

Another way, for a method that is easier to automate, but harder for users to execute:

1. Copy the file to `%USERPROFILE%\.nrfconnect-apps\local` (Windows) or
   `$HOME/.nrfconnect-apps/local` (Linux or macOS).
2. Restart nRF Connect for Desktop (Ctrl-R on Windows or Linux, Cmd-R on macOS).
   The app should now appear in the apps list.

**Note:** If the app has the same name as an official app, it will appear twice in the
list. You can differentiate the two by the label below it ("local" vs "official"):

![nRF Connect for Desktop launcher with "local" and "official" app versions](./multiple_versions_in_launcher.png 'nRF Connect for Desktop launcher with "local" and "official" app versions')
