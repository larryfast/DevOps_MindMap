### database updates
- Apps should be as stateless as possible
- Push all persistent data into a DB
- Persistent data is handled differently than stateless app services
	- Updates cannot replace the data component of the server
	- still possible to replace the DB 'server' when the data is on an attached partition
	- harder to build canary or blue-green deploys
- Changes must be [[Backward Compatible]]
	- If not, the changes get coupled to simultaneous updates of dependent system components