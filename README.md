# cli-task-manager

## A command-line application to manage tasks (TODOs) with add/list/edit/complete/delete/search features, persisted to disk. Focus on idiomatic modern C++ (C++17 or later), good code organization, and unit tests.

- Inputs: user text commands via CLI and a persistent tasks file (e.g., tasks.json or tasks.csv).
- Outputs: printed lists to stdout, updated file on disk, program exit status (0 on success).
- Data shape: A Task { id: int, title: string, description: optional string, tags: vector<string>, due: optional date/time, completed: bool }.
- Error modes: invalid command syntax (print usage), file I/O errors (print message and nonzero exit if fatal), malformed data file (fail gracefully with option to reset).