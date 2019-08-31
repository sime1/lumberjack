# Lumberjack

Lumberjack provides a rolling logger.

Lumberjack plays well with any logging package that can write to an
io.Writer, including the standard library's log package.

Lumberjack assumes that only one process is writing to the output files.
Using the same lumberjack configuration from multiple processes on the same
machine will result in improper behavior.

This fork adds the ability to specify a different directory for the backup
log files. It also changes how the logger is created, to improve the way default
parameters are used.
