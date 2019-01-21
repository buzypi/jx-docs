---
date: 2019-01-21T16:11:15Z
title: "jx create user"
slug: jx_create_user
url: /commands/jx_create_user/
---
## jx create user

Create a new User which is then provisioned by the user controller

### Synopsis

Creates a user

```
jx create user [flags]
```

### Examples

```
  # Create a user
  jx create user -e "user@email.com" --login username --name username"
```

### Options

```
  -b, --batch-mode                In batch mode the command never prompts for user input
  -e, --email string              The users email address
      --headless                  Enable headless operation if using browser automation
  -h, --help                      help for user
      --install-dependencies      Should any required dependencies be installed automatically
      --log-level string          Logging level. Possible values - panic, fatal, error, warning, info, debug. (default "info")
  -l, --login string              The user login name
  -n, --name string               The textual full name of the user
      --no-brew                   Disables the use of brew on macOS to install or upgrade command line dependencies
      --pull-secrets string       The pull secrets the service account created should have (useful when deploying to your own private registry): provide multiple pull secrets by providing them in a singular block of quotes e.g. --pull-secrets "foo, bar, baz"
      --skip-auth-secrets-merge   Skips merging a local git auth yaml file with any pipeline secrets that are found
      --verbose                   Enable verbose logging
```

### SEE ALSO

* [jx create](/commands/jx_create/)	 - Create a new resource

###### Auto generated by spf13/cobra on 21-Jan-2019