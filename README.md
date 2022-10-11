# Plugin Encryption Tool

This is a QSC tool you can use to encrypt your Q-SYS Plugin source code. This can ensure protection of any ids, keys, or intellectual property you might not want to be made publicly available.

## Using the Tool in Windows PowerShell

To use this tool, navigate to the folder with the plugin_tool_release.exe on your local machine.

Launch PowerShell by holding shift and right clicking. Select 'Open PowerShell window here'.

To access the commands for the tool, use the syntax ./plugin_tool_release.exe <your_command_here>

### Encryption Tool Commands

**usage**   : returns the currently supported commands and their syntax. Please note that invalid commands or a blank command will return the same as the **usage** command.

**version** : returns the current version for the tool

**encrypt** : encrypts the specified input file and outputs it to the specified output file. 
              For example: ./plugin_tool_release.exe encrypt MyPlugin.qplug MyEncryptedPlugin.qplugx
  
Please note that encrypted plugins have the 'qplugx' extension. Additionally, if the file you are attempting to encrypt is not in the same folder as the tool, you'll need to specify the file location. 

For example: ./plugin_tool_release.exe encrypt C:\<path_to_your_plugin>\ATestPlugin.qplug C:\<path_to_your_plugin>\ATestPlugin\ATestPlugin.qplugx

## Support

If you have any questions or concerns, please contact qsyscontrolfeedback@qsc.com