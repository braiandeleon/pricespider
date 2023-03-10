HOWDY!

If you are reading this, there are a few things you'll need to change
within this folder before you're able to use it.

First, please re-name the .config files within the Automatch folder.
* appSettings.mquinlan.config -> appSettings.yourNameHere.config
		Note: CASE MATTERS (stay lower case to make it simple)
* connectionstrings.mquinlan.config -> connectionstrings.yourNameHere.config

Secondly, open the first file we renamed [appSettings.mquinlan.config] and rename
the following values:
* <add key="processID" value="mquinlan"/> [mquinlan -> yourNameHere]
* <add key="webserverid" value="mquinlan" /> [mquinlan -> yourNameHere]

Finally, open the file named [AutoMatchTestHarness.exe.config] NOT the .exe file.
* <connectionStrings configSource="connectionStrings.mquinlan.config"></connectionStrings>
	[mquinlan -> yourNameHere]
* <appSettings configSource="appSettings.mquinlan.config"></appSettings>
	[mquinlan -> yourNameHere]

NOTE: CASING MATTERS!!! so mquinlan != mQuinlan


If you are still experiencing issues, please reach out to your team lead/manager for assistance.