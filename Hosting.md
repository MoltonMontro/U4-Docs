# Hosting

Downloading the dedicated server from the tools tab requires a login during the private beta, but will be available anonymously once the game is marked as released on Steam.

Running a client on the same machine as dedicated server(s) requires specifying the -DisableSteamServerInit launch option. Running a listen server does not require this however.

Launch the server with the map name, and -Log to open a command prompt. Valid map names:

	Firing_Range
	Blastlane
	Survival_Sandbox
	Horde_Sandbox
	Horde_Chapel
	Horde_Potato

Until configuration is thoroughly implemented, a temporary config file format similar to 3.0's is available. Specify the -U4SV=MyFile.ini on the command-line. This can be a file name in the Saved folder, or an absolute file path anywhere on the system. The game populates defaults in this format:

	[OnlineSession]
	OnlineSession="Name in the server list"
	MaxPlayers=64
	MaxSpectators=2

	[Whitelist]
	UniqueNetIds=STEAM:FirstSteamId64
	UniqueNetIds=STEAM:SecondSteamId64
