<img src="icon/icon_round.png" width="76"/>

# Pass
[![GitHub release](https://img.shields.io/github/release/mssun/passforios.svg)](https://github.com/mssun/passforios/releases)
[![Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/passforios/passforios)
[![Build Status](https://travis-ci.org/mssun/passforios.svg?branch=develop)](https://travis-ci.org/mssun/passforios)
[![Donate](https://img.shields.io/badge/paypal-donate-blue.svg)](https://www.paypal.me/mssun)

Pass is an iOS client compatible with [ZX2C4's Pass command line application](http://www.passwordstore.org/).
It is a password manager using GPG for encryption and Git for version control.

Pass for iOS is available in App Store with the name "Pass - Password Store", and both iPhone and iPad are supported.

<p>
<a href="https://itunes.apple.com/us/app/pass-password-store/id1205820573?mt=8"><img alt="Download on the App Store" src="img/app_store_badge.svg" width="150"/></a>
</p>

You can also help us test beta versions through [TestFlight](https://testflight.apple.com/join/whK4zUFG).

## Features

- Compatible with the Password Store command line tool.
- View, copy, add, and edit password entries.
- Encrypt and decrypt password entries by PGP keys.
- Synchronize with your password Git repository.
- User-friendly interface: search, long press to copy, copy and open link, etc.
- Support one-time password tokens (two-factor authentication codes).
- Autofill in Safari/Chrome and [supported apps](https://github.com/agilebits/onepassword-app-extension).

## Screenshots

<p>
<img src="img/screenshot1.png" width="200"/>
<img src="img/screenshot2.png" width="200"/>
<img src="img/screenshot3.png" width="200"/>
<img src="img/screenshot4.png" width="200"/>
</p>

## Usages

- Setup your password-store ([official `Pass` introduction](https://www.passwordstore.org/))
- Get Pass for iOS from the App Store or [build by yourself](https://github.com/mssun/passforios/wiki/Building-Pass-for-iOS)
- Setup Pass for iOS ([quick-start guide](https://github.com/mssun/passforios/wiki#quick-start-guide-for-pass-for-ios))

For more, please read the [wiki page](https://github.com/mssun/passforios/wiki).

## Building Pass for iOS

1. Install libtool, automake, cmake, carthage, cocoapods, and go: `brew install libtool automake cmake carthage cocoapods go`.
2. Install dependencies via Carthage in the project root directory: `./wcarthage update` then `./wcarthage bootstrap --platform iOS`. This may take some time.
3. Run `./gopenpgp_build.sh` to build go dependencies.
4. Install dependencies via CocoaPods in the project root directory: `pod install`.
5. Open the `pass.xcworkspace` file in Xcode.
6. Build & Run.

## License

MIT
