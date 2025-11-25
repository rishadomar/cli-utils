# Useful cli utilities

### Installation

1. git clone in some bin folder
2. chmod +x the files

Examples:

### List changes made

git-changes --since '1 week ago'
git-changes --author rishad --since yesterday
git-changes --author rishad --since '1 week ago' --brief

### List MY changes

This requires you to edit the git-my-changes utility:

-   list your repositories for which you want a log
-   add your personal arguments like: ARGS=(--author rishad --since "1 week ago" --brief)
