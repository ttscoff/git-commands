# Brett's Git Commands

Just some simple git commands that made more sense as
scripts than as aliases.

## Installation

Clone this repo and copy or link the directory into your
$PATH and call them like `git ar` or `git finda ci`. Make
sure the scripts are executable.

More complex commands will display usage instruction
with `-h`.

## Dependencies

Some scripts require external tools:

- [gum]
- [fzf]
- [hub] or [gh]

All easily installed with Homebrew.

## Commands

- `git ar` - Add all new files to staging and remove deleted files
- `git comm [<summary>]` - Pretty commit message input using [gum]
- `git finda [<alias>]` - Find a git alias using pattern matching
- `git ig [<lang>]` - Add contents of an ignore file from gitignore.io, uses [fzf]
- `git iglist` - List all available ignore files
- `git logjson` - Output a JSON-formatted git log
- `git releasenext [major|minor|*patch]` - Creates a release using [hub] or [gh] for the next semantic version (based on tags)
- `git semnext [major|minor|*patch]` - Output the next semantic version number
- `git sign` - Enable/disable GPG signing, assign key for repo or globally
- `git ver` - Display the current semantic version (based on tags)
- `git whyig` - Show ignored files and explain why/how they're ignored

[gum]: https://github.com/charmbracelet/gum
[fzf]: https://github.com/junegunn/fzf
[hub]: https://github.com/mislav/hub
[gh]: https://cli.github.com/

## Aliases

`useful-git-aliases.conf` contains a collection of useful aliases.

### Usage

Save `useful-git-aliases.conf` somewhere on your system. I
like to put it in a folder I sync with Dropbox between my
machines:

     ~/.local/share/git/useful-git-aliases.conf

Edit ~/.gitconfig to include this file:

     vim ~/.gitconfig

Include the path to the alias file:

    [include]
    path = ~/.local/share/git/useful-git-aliases.conf

The file includes some aliases from [@durdn](https://www.durdn.com/blog/2012/11/22/must-have-git-aliases-advanced-examples/).


Once installed, `git la` will list all your aliases.

## License

This repo is licensed under the MIT License.

See <https://opensource.org/licenses/MIT> for details.
