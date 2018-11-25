[![appveyor build](https://ci.appveyor.com/api/projects/status/github/bitwarden/desktop?branch=master&svg=true)](https://ci.appveyor.com/project/bitwarden/desktop)
[![travis build](https://travis-ci.org/bitwarden/desktop.svg?branch=master)](https://travis-ci.org/bitwarden/desktop)
[![Crowdin](https://d322cqt584bo4o.cloudfront.net/bitwarden-desktop/localized.svg)](https://crowdin.com/project/bitwarden-desktop)
[![Join the chat at https://gitter.im/bitwarden/Lobby](https://badges.gitter.im/bitwarden/Lobby.svg)](https://gitter.im/bitwarden/Lobby)

# Bitwarden Desktop Application

[![Platforms](https://imgur.com/SLv9paA.png "Windows, macOS, and Linux")](https://bitwarden.com/#download)

The Bitwarden desktop app is written using Electron and Angular. The application installs on Windows, macOS, and Linux distributions.

![Desktop Vault](https://raw.githubusercontent.com/bitwarden/brand/master/screenshots/desktop-macos-vault.png "My Vault")

# Build/Run

**Requirements**

- [Node.js](https://nodejs.org/)
- Windows users: To compile the native node modules used in the app you will need the Visual C++ toolset, available through the standard Visual Studio installer (recommended) or by installing [`windows-build-tools`](https://github.com/felixrieseberg/windows-build-tools) through `npm`. See more at [Compiling native Addon modules](https://github.com/Microsoft/nodejs-guidelines/blob/master/windows-environment.md#compiling-native-addon-modules).

**Compile the app**
```bash
git clone --recursive https://github.com/h44z/desktop.git Bitwarden-Desktop
cd Bitwarden-Desktop

npm install

cd jslib
npm install
cd ..

# To start the app run
npm run electron

# To just build the app run
npm run build
```

**Run the app**

```bash
npm install
npm run electron
```

# Contribute

Code contributions are welcome! Please commit any pull requests against the `master` branch. Learn more about how to contribute by reading the [`CONTRIBUTING.md`](CONTRIBUTING.md) file.

Security audits and feedback are welcome. Please open an issue or email us privately if the report is sensitive in nature. You can read our security policy in the [`SECURITY.md`](SECURITY.md) file.
