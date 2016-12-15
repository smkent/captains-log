`captains-log` is a simple daily personal logging application designed to store
short notes about each day in plain text.

The log is stored as individual files named for the corresponding date within a
`git` repository. Each addition or modification to the log also creates a
new commit in order to preserve the entire history of the log.

## Usage

`captains-log` organizes its main actions into commands, similar to `git`.
The available commands are `read`, `write`, `search`, and `history`.

A few shortcuts are available without specifying a command, such as being able
to simply enter a note into the current day's log by invoking `captains-log`
followed by text on the command line.

| Action | Example command |
| :-- | :-- |
| Write to the log for today | `$ captains-log Text to enter into the log` |
| Open `$EDITOR` to compose/edit today's log | `$ captains-log` |
| Edit the log entry for the previous day | `$ captains-log -d yesterday` |
| Show all log entries in reverse chronological order | `$ captains-log read` |
| Show just the log entry for today | `$ captains-log read today` |
| `grep` for a particular word in the log | `$ captains-log search text` |

Full usage information is available by running `captains-log --help`, or
`captains-log [command] --help` for information about a specific command.

## License

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

See [`LICENSE`](/LICENSE) for the full license text.
