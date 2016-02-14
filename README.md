# Google's V8 Javascript engine (for embedding)

## V8 v4.10 (candidate)

Currently, only Win64 binaries (both Debug and Release versions) have been uploaded. 

Built with VS2013, with the following GYP flags
- `-Dcomponent=shared_library`
- `-Dv8_enable_disassembler=0`
- `-Dv8_use_snapshot=0`
- `-Dv8_enable_gdbjit=0`
- `-Dv8_enable_i18n_support=0`
- `-Dv8_enable_handle_zapping=0`

