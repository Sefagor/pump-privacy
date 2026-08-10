# pump-privacy

Public hosting for the [Pump](https://play.google.com/store) privacy policy, served by GitHub Pages
at **https://sefagor.github.io/pump-privacy/privacy.html**.

This repo exists only because GitHub Pages will not serve a private repository on the free plan, and
the Pump app repo is private. Nothing here is application code.

## Do not edit `privacy.html` here

The source of truth is `docs/privacy.html` in the **PumpKotlin** repo. Edit it there, then copy the
file across and push. Editing this copy directly means the two drift, and Play compares the live
policy against the Data Safety answers derived from the app.

The URL is compiled into the app at `AboutScreen.kt` (`PRIVACY_POLICY_URL`) and is filed in Play
Console as both the privacy policy URL and the account-deletion URL, so **it must not change** once
a build has shipped.

## Licence

Intentionally none. This repository contains a legal document, not source code — there is no reason
to grant redistribution or modification rights over Pump's privacy policy, and an open-source licence
here would also blur the proprietary status of the (private) app repo. All rights reserved by
default.

© 2026 PumpHQ. All rights reserved.
