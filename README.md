# Google's V8 Javascript engine binaries for embedding

## V8 v4.10 (candidate)

Currently, only Win64 binaries (both Debug and Release versions) have been uploaded. If I manage to build it on other platforms, I'll upload the binaries here.

Built with VS2013, with the following GYP flags
- `-Dcomponent=shared_library`
- `-Dv8_enable_disassembler=0`
- `-Dv8_use_snapshot=0`
- `-Dv8_enable_gdbjit=0`
- `-Dv8_enable_i18n_support=0`
- `-Dv8_enable_handle_zapping=0`

You can download a zip package containing all the files (~32MB) or only the files you are interested in. I've also included .pdb's but I don't know if they are useful without the source. Finally, d8.exe and shell.exe are included.

If you can't make them link correctly with your app, or if you want to build V8 with a different set of flags, you can always try building from sources :) If you are on Windows, don't forget to `set DEPOT_TOOLS_WIN_TOOLCHAIN=0` before running `gyp_v8` (as it's described here: [https://www.chromium.org/developers/how-tos/build-instructions-windows](https://www.chromium.org/developers/how-tos/build-instructions-windows)

Have fun!
