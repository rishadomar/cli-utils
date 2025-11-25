# Useful cli utilities

### Installation

1. git clone in some bin folder
2. chmod +x the files

Examples:

### List changes made in the current repo

-   List changes made by all users in the last week
    `git-changes --since '1 week ago'`

-   List changes made by me today
    `git-changes --author $USERNAME --since yesterday`

-   List changes made by specific user (brief mode)
    `git-changes --author ahmed --since '1 week ago' --brief`

### List MY changes in all the repos that I specify

This requires you to edit the git-my-changes utility and the paths of repositories for which you want a log

-   List all the changes made by me today
    `git-my-changes`

-   List all the changes made by me in the last week
    `git-my-changes --since '1 week ago'`
