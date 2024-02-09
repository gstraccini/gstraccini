# GStraccini GitHub Bot

🤖 :octocat: A GitHub bot that runs on issues, pull requests, and pull request comments.

## Useful links

- GitHub App: https://github.com/apps/gstraccini
- Bot's site: https://bot.straccini.com/
- Source code: https://github.com/guibranco/gstraccini-bot

## What this bot can do

That's what I can do :neckbeard::
- `@gstraccini help`: Shows the help message with available commands.
- `@gstraccini hello`: Says hello to the invoker.
- `@gstraccini thank you`: Replies with you are welcome message to the invoker.
- `@gstraccini appveyor <type>`: Runs the [AppVeyor](https://ci.appveyor.com) build for the target commit and/or pull request
	- `type`: `[required]` Specifies if it should trigger a build in a `commit` or `pull request`.
- `@gstraccini bump version <version> <project>`: Bumps the [.NET version](https://dotnet.microsoft.com/en-us/platform/support/policy/dotnet-core) in .csproj files. :warning: (in development - maybe not working as expected!)
	- `version`: `[required]` The .NET version
	- `project`: `[optional]` The `.csproj` file to update. Suppressing this parameter will run the command in all `.csproj` in the repository/branch
- `@gstraccini change runner <runner> <workflow> <jobs>`: Changes the [GitHub action runner](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners/about-github-hosted-runners#supported-runners-and-hardware-resources) in a workflow file (.yml) :warning: (in development - maybe not working as expected!)
	- `runner`: `[required]` The runner's name
	- `workflow`: `[required]` The workflow filename (with or without the .yml/.yaml extension)
	- `jobs`: `[optional]` The job's to apply this command. Suppressing this parameter will run the command in all jobs within the workflow
- `@gstraccini csharpier`: Formats the C# code using [CSharpier](https://csharpier.com) (only for **.NET** projects).
- `@gstraccini fix csproj`: Updates the `.csproj` file with `packages.config` version of [NuGet packages](https://nuget.org) (only for **.NET Framework** projects). :warning: (in development - maybe not working as expected!)
- `@gstraccini prettier`: Formats the code using [Prettier](https://prettier.io).
- `@gstraccini review`: Enable review for the target pull request. This is useful when the PR submitter wasn't on the watch list before, the webhook was not captured, or some failed scenario occurred.
- `@gstraccini track`: Tracks the specified pull request. Queue a build, raise a **[dependabot](https://github.com/dependabot) recreate** comment to resolve conflicts and synchronize merge branches. :warning: (in development - maybe not working as expected!)


Multiple commands can be issued at the same time. Just respect each command pattern (with bot name prefix + command).

> **Warning**
> 
> If you aren't allowed to use this bot, a reaction with a thumbs down will be added to your comment.


## Maintainer 

This account, bot, app and site are maintained by [@GuiBranco](https://github.com/guibranco)
