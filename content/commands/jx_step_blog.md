---
date: 2019-01-21T16:11:15Z
title: "jx step blog"
slug: jx_step_blog
url: /commands/jx_step_blog/
---
## jx step blog

Creates a blog post with changes, metrics and charts showing improvements

### Synopsis

Generates charts for a project

```
jx step blog [flags]
```

### Examples

```
  # create charts for the cuect
  jx step chart
```

### Options

```
  -b, --batch-mode                 In batch mode the command never prompts for user input
      --blog-dir string            The Hugo-style blog source code to generate the charts into
  -n, --blog-name string           The blog name
  -c, --combine-minor              If enabled lets combine minor releases together to simplify the charts (default true)
      --dev-channel-members int    If no chat bots can connect to your chat server you can pass in the counts for the developer channel here
  -d, --dir string                 The directory to query to find the projects .git directory
  -f, --from-date string           The date to create the charts from. Defaults to a week before the to date. Should be a format: January 2 2006
      --headless                   Enable headless operation if using browser automation
  -h, --help                       help for blog
      --install-dependencies       Should any required dependencies be installed automatically
      --log-level string           Logging level. Possible values - panic, fatal, error, warning, info, debug. (default "info")
      --no-brew                    Disables the use of brew on macOS to install or upgrade command line dependencies
      --pull-secrets string        The pull secrets the service account created should have (useful when deploying to your own private registry): provide multiple pull secrets by providing them in a singular block of quotes e.g. --pull-secrets "foo, bar, baz"
      --skip-auth-secrets-merge    Skips merging a local git auth yaml file with any pipeline secrets that are found
  -t, --to-date string             The date to query up to. Defaults to now. Should be a format: January 2 2006
      --user-channel-members int   If no chat bots can connect to your chat server you can pass in the counts for the user channel here
      --verbose                    Enable verbose logging
```

### SEE ALSO

* [jx step](/commands/jx_step/)	 - pipeline steps

###### Auto generated by spf13/cobra on 21-Jan-2019