<img src="banner.svg" width="22%" align="right">

Serve
=====
Bundle any script as a macOS _[service]_.

[CLI]
-----
`serve script` [`--icon icon`]

| Flag | Long        | Description                                             |
|:-----|:------------|:--------------------------------------------------------|
| `-h` | `--help`    | Print brief usage information.                          |
| `-v` | `--version` | Print running version info.                             |
| `-i` | `--input`   | Type of input the service should accept.                |
| `-a` | `--app`     | Limit access to service only from within the given app. |
| `-n` | `--icon`    | Apply icon from any image or icon file.                 |
| `-m` | `--install` | Compile service into `~/Library/Services`.              |

`serve script.sh --icon *.icns`

Install
-------
with _[Homebrew]_:
~~~ sh
brew tap max-os/{install,services}
brew install serve
#brew cask install serve
~~~

Development
-----------
~~~ sh
git clone https://github.com/max-os/serve.git
cd serve
brew bundle
git config core.hooksPath hooks
~~~

Part of _[maxOS]_.

License
-------
[MIT] © [Daniel Bayley]

[MIT]:              LICENSE.md
[Daniel Bayley]:    https://github.com/danielbayley

[service]:          https://developer.apple.com/macos/human-interface-guidelines/extensions/services

[maxos]:            http://max-os.github.io
[cli]:              man.md

[homebrew]:         http://brew.sh
