# Bus Riders United STL Website
This is the source code for the Bus Riders United STL Website.
Built using [Hugo](gohugo.io) and hosted via GitHub pages.

# Getting Started

## Prerequsites
- [Hugo](https://gohugo.io/getting-started/installing/)

## Setup
- Run this command inside the repository to set up the git hooks -
`git config --local hooks.corePath .githooks`

## Basic Development Flow
- You can spin up a development server of the site by running `hugo server`, which will automatically reload when any changes happen
	- You can also run `hugo server -D` which will do the same thing, but display drafts, which is great for developing
- When you commit your changes, the Git hook will automatically run `hugo` to build the site, and add that to your commit, so you'll always commit the newest version of the built site!


# Repo Structure

- `archtypes/` - Defines default values for new posts
- `config.toml` - Main configuration for the site
- `content/` - Markdown files that define posts, pages, etc.
- `docs/` - The generated site that gets published. 
	- This is confusingly named -- GitHub pages requires that you publish
	from either a different branch or the `docs/` folder, and publishing
	from a separate branch is a bit more work.
- `themes/` - Contains Hugo themes, which define styles and layout of the site.
- `.githooks/` - Contains scripts that run after git events
