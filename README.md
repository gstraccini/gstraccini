# GStraccini GitHub Bot

🤖 :octocat: A GitHub bot that runs on issues, pull requests, and pull request comments.

## Useful links

- GitHub App: https://github.com/apps/gstraccini
- Bot's site: https://bot.straccini.com/
- Source code: https://github.com/guibranco/gstraccini-bot

## What this bot can do

That's what I can do :neckbeard::

@gstraccini help: Shows the help message with available commands.
@gstraccini hello: Says hello to the invoker.
@gstraccini thank you: Replies with you are welcome message to the invoker.
@gstraccini appveyor <type>: Runs the AppVeyor build for the target commit and/or pull request
type: [required] Specifies if should trigger a build in a commit or pull request.
@gstraccini bump version <version> <project>: Bumps the .NET version in .csproj files. ⚠️ (in development - maybe not working as expected!)
version: [required] The .NET version
project: [optional] The .csproj file to update. Suppressing this parameter will run the command in all .csproj in the repository/branch
@gstraccini change runner <runner> <workflow> <jobs>: Changes the GitHub action runner in a workflow file (.yml) ⚠️ (in development - maybe not working as expected!)
runner: [required] The runner's name
workflow: [required] The workflow filename (with or without the .yml/.yaml extension)
jobs: [optional] The job's to apply this command. Suppressing this parameter will run the command in all jobs within the workflow
@gstraccini csharpier: Formats the C# code using CSharpier (only for .NET projects).
@gstraccini fix csproj: Updates the .csproj file with packages.config version of NuGet packages (only for .NET Framework projects). ⚠️ (in development - maybe not working as expected!)
@gstraccini prettier: Formats the code using Prettier.
@gstraccini review: Enable review for the target pull request. This is useful when the PR submitter wasn't in the watch list before or the webhook was not captured or some failed scenario occurred.
@gstraccini track: Tracks the specified pull request. Queue a build, raise dependabot recreate comment to resolve conflicts and synchronize merge branches. ⚠️ (in development - maybe not working as expected!)
Multiple commands can be issued at the same time, just respect each command pattern (with bot name prefix + command).

Warning

If you aren't allowed to use this bot, a reaction with a thumbs down will be added to your comment.

## Maintainer 

This account, bot, app and site are maintained by [@GuiBranco](https://github.com/guibranco)
