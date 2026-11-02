# PluginTool

This is a QSC tool you can use to encrypt your Q-SYS Plugin source code.

## Usage

```plugin_tool.exe {help|-h|--help|?}```

```plugin_tool.exe encrypt {-i|--input-file} <input_file> [{-o|--output-file} <output_file>] [{-m|--mode} {CoreOnly|CoreAndEmulate|CoreOnlyV3|CoreAndEmulateV3|Legacy}```

### Notes

- Powershell is suggested for use of this tool.
- If output-file is not provided it will use the same file name with the corresponding extension
  - .qplugx for Legacy
  - .qplugx2 for CoreAndEmulate or CoreOnly
- mode will default to CoreAndEmulate
- arguments can be passed in in any order after encrypt, for example:
  - plugin_tool.exe encrypt -i MyPlugin.qplug -m Legacy
  - plugin_tool.exe encrypt -m Legacy -i MyPlugin.qplug

## Modes

### Legacy

Will run in all versions of QSYS Designer that support encrypted plugins.

### CoreAndEmulate (Default)

Will only run in Q-SYS Designer 9.10 and later.

### CoreAndEmulateV3

Will only run in Q-SYS Designer 10.5 and later.

### CoreOnly

Same as CoreAndEmulate but the runtime code is only decoded on a QSYS Core. The Plugin will report Fault in Emulation.

### CoreOnlyV3

Same as CoreOnly but requires Q-SYS Designer 10.5 and later.

## Support

If you have any questions or concerns, please go to [support.qsys.com/contact-us](https://support.qsys.com/contact-us)
