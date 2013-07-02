**Distribution files for Telefonica customization build**

We have not (fully) supported preload apps, so please copy external-apps/* to GAIA_DIR/external-apps.

 - Note: For Gaia master (with [Gaia commit 316ca1ee](https://github.com/mozilla-b2g/gaia/commit/316ca1ee98d2f813f5605c7deb87f6e9d4465df6)), you don't have to do the above manual copy.
 - See [Bug 838098](https://bugzilla.mozilla.org/show_bug.cgi?id=838098) - Install the apps, external apps in customization package for details.

Instructions
============

just clone this repository, copy external-apps and make your production build
with official branding!

    $ git clone git://github.com/telefonicaid/firefoxos-gaia-spain.git <DIST_DIR>
    $ cp -r <DIST_DIR>/external-apps/* <GAIA_DIR>/external-apps/
    $ MOZILLA_OFFICIAL=1 GAIA_DISTRIBUTION_DIR=<DIST_DIR> make production
