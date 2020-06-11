# Release Note Generator

This command line utility will generate release notes based on the commit messages

## How it works

It will

- Compare the live and master branches
- Find JIRA ticket references in the commits
- Fetch the JIRA ticket titles from JIRA
- Generate a Markdown list of all the tickets that have been affected

## Running the utility

`npx @goodcity/release-notes`

### Options

```bash
$> npx @goodcity/release-notes --help

Usage: @goodcity/release-notes [options]

Options:
  -V, --version              output the version number
  -p, --pdf                  ouputs to pdf
  -c, --clipboard            copies the markdown to your clipboard
  -h, --head <head>          The head ref or source branch (default: "origin/master")
  -b, --base <base>          The base ref or target branch (default: "origin/live")
  --email-to <email>         Recipients for the release notes
  --email-subject <subject>  Subject of the email
  --help                     display help for command
```

