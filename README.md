# USGS Data Science tutorial for Git and GitHub workflow

This template repository contains the issues and starting content to teach the DS fork-and-pull style workflow. For the full experience, it requires someone else (listed as @lindsayplatt in these instructions) to review and merge your pull requests. 

## I'm a learner

Go to the repo that matches your username, `USGS-R/ds-gitflows-[username]`.

## I'm leading the course

1. Create a new repository based on this template repo using the naming convention `ds-gitflows-[username]` for each participant. These will be considered the canonical repository for each participant.
1. Go to each of these new repositories you just made and star them. This will manually trigger the workflow that creates the necessary GitHub issues to complete the training using GitHub actions.
1. Give each participant `triage` access to their repository. This will allow them to make PRs and close issues, but will prevent them from being able to write directly to the master repository. The participant will need to accept the invitation. The only other caveat is that `triage` access may make it so that they need to create a pull request before seeing the option to assign a reviewer. This was the case for someone who was not part of the `USGS-R` organization but tested the repo.
1. Be prepared to review and merge 3 pull requests per participant (one with their first two commits, one with merge conflicts resolved, one with changes to the `.gitignore` file).
1. The rest of the course should run automatically.
