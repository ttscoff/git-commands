# Brett's Git Commands

Just some simple git commands that made more sense as
scripts than as aliases.

## Installation

Copy or link these files into your PATH and call them like
`git ar` or `git finda ci`. Make sure the scripts are
executable.

More complex commands will display usage instruction with `-h`.

## Dependencies

Some scripts require external tools:

- [gum]
- [fzf]
- [hub]

All easily installed with Homebrew.

## Commands

- `git ar` - Add all new files to staging and remove deleted files
- `git comm [<summary>]` - Pretty commit message input using [gum]
- `git finda <alias>` - Find a git alias using pattern matching
- `git ig [<lang>]` - Add contents of an ignore file from gitignore.io, uses [fzf]
- `git iglist` - List all available ignore files
- `git logjson` - Output a JSON-formatted git log
- `git releasenext [major|minor|*patch]` - Creates a release using [hub] for the next semantic version (based on tags)
- `git semnext [major|minor|*patch]` - Output the next semantic version number
- `git sign` - Enable/disable GPG signing, assign key for repo or globally
- `git ver` - Display the current semantic version (based on tags)
- `git whyig` - Show ignored files and explain why/how they're ignored

[gum]: https://github.com/charmbracelet/gum
[fzf]: https://github.com/junegunn/fzf
[hub]: https://github.com/mislav/hub