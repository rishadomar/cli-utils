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

### Generate AI-powered release notes from commits

This requires a Gemini API key (free from https://aistudio.google.com/apikey)

Setup:

```bash
export GEMINI_API_KEY='your-api-key-here'
# Add to ~/.bashrc for persistence
```

-   Generate release notes from a tag/branch to current state
    `git-release-notes --from v1.2.0`

-   Generate release notes between two branches
    `git-release-notes --from main --to develop`

-   Save release notes to a file
    `git-release-notes --from v1.0.0 --output RELEASE_NOTES.md`

-   Verbose output to see processing details
    `git-release-notes --from release/1.0 --verbose`
