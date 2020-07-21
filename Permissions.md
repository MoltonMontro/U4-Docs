# Permissions

For the meantime permissions are loaded from the per-server ini file, for example:

	[Permissions]
	DefaultRole=MyFirstRole
	Roles=MyFirstRole
	Roles=MySecondRole

	[MyFirstRole]
	Permissions=u4.help

	[MySecondRole]
	Permissions=u4.role
	Permissions=u4.spawn_item
	Members=MySteamId
	Members=AnotherSteamId

The role command can also be used to add permissions and members to roles. It writes to the ini file.

## Future Work

- Reading and writing roles from separate ini files.
- Alternative role backends e.g. database.
- Parent roles and inheritance.
