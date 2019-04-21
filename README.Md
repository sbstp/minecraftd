# minecraftd
A supervisor for the Minecraft process. Avoids corruption of the world data files.

### Why?
* Clean shutdowns: Catches SIGINT & SIGTERM and issues a stop command to the minecraft server for a clean shutdown.
* Clean backups: Disables auto-save, flushes all the pending changes, makes a backup and then enables auto-save.
