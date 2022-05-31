# Connecting to a service with passkeys

Allow users to sign in to a service without typing a password.

## Overview

- Note: This sample code project is associated with WWDC22 session [10092: Meet passkeys](https://developer.apple.com/wwdc22/10092/) and WWDC21 session [10106: Move beyond passwords](https://developer.apple.com/wwdc21/10106/).


## Configure the sample code project

To build and run this sample:
1. Open the sample with Xcode 14 or later.
2. Select the Shiny project.
3. For the project's target, select your team from the Team drop-down menu in the Signing & Capabilities pane to let Xcode automatically manage your provisioning profile.
4. Add the Associated Domains capability using the "+ Capability" button in the same pane, and specify your domain with the `webcredentials` service.
5. Ensure an `apple-app-site-association` (AASA) file is present on your domain in the `.well-known` directory, and that it contains an entry for this app's App ID for the `webcredentials` service.
6. In the `AccountManager.swift` file, replace all occurrences of `example.com` with the name of your domain.
