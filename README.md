<h1 align="center">Carthage Helper</h1>
<pre align="center">
A ruby script that helping you import third-party frameworks that manager by Carthage
</pre>

Components of [XcodeScriptsKit](https://github.com/CodeEagle/XcodeScriptsKit)

Features
---
- [x] import frameworks in `Carthage/Build/iOS` folder to your targets in `path/to/your/*.xcodeproj`
- [x] adjust project deployment target to `iOS 9.0`
- [x] shared `Framework`(aka `FMWK`) target scheme by default
- [x] add copy script phase for Application(aka `APPL`) target, turn off system log on by adding `OS_ACTIVITY_MODE`
- [x] add copy file phase for `Unit Test`(aka `BNDL`) target
- [x] optional skip certain target (only one)
- [x] add search path for each target
- [x] backup `*.xcodeproj` once in folder `project_backup`

Installtion
---
- Jsut download the `carthage_helper.rb` file.

- add alias in your `~/.zshrc` file

  `alias carthelper='ruby path/to/your/carthage_helper.rb $(pwd)'`

⚠️Caveat
---
- If something went wrong, retrieve backup form `project_backup`.
- [New issue](https://github.com/CodeEagle/CarthageHelper/issues) here

Usage
---
`cd path/to/your/*.xcodeproj && carthelper`


Wiki
---
There has 2 parameters need to pass to the script

1. `path/to/your/*.xcodeproj`
2. target name that need skipping(only one target)
