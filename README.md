# CoreAudioSDK
Here's the definitive source of the Core Audio SDK because Apple doesn't care to provide one.
Originally from Apple documentation Archive, [Core Audio Utility Classes](https://developer.apple.com/library/archive/samplecode/CoreAudioUtilityClasses/Introduction/Intro.html).

## What's different

#### `verify` and `verify_noerr`
These macros are removed by Apple in macOS 10.13 ([Source](https://github.com/cebix/macemu/issues/141#issuecomment-336256848)).
They are replaced with `__Verify` and `__Verify_noErr` so the code would compile under the latest macOS.

#### Carbon things (`.r` files)
I have no idea how to deal with Carbon and I never used these to develop graphical AU plugin,
so I didn't include any of the `.r` files in the targets.
If you are familiar with Carbon please make PRs ❤️

