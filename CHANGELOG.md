# Unreleased

## Added
* Added `set_bitrate` method to dynamically change encoder bitrate during encoding

## Changed
* Replaced `env-libvpx-sys` with `libvpx-native-sys` to resolve build failures on macOS environments
* Removed `ffi-generate` feature as it's no longer needed with the new dependency

# 0.5.0 - 2021-06-07

## Changed
* `Error` type is now a struct with a message and a, optionally, a backtrace. To
  get backtraces, use the `backtrace` cargo feature. (Currently, nightly rust is
  required for this feature.)