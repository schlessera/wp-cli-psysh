schlessera/wp-cli-psysh
=======================

Replace WP-CLI shell standard REPL with PsySH.



Quick links: [Using](#using) | [Installing](#installing) | [Contributing](#contributing) | [Support](#support) | [How it Works](#how-it-works)

## Using

There's not much to do here. As soon as you install this additional package, the default `wp shell` REPL will be replaced with the awesome [PsySH](http://psysh.org/).

## Installing

Installing this package requires WP-CLI v1.1.0 or greater. Update to the latest stable release with `wp cli update`.

Once you've done so, you can install this package with:

    wp package install git@github.com:schlessera/wp-cli-psysh.git

## Contributing

We appreciate you taking the initiative to contribute to this project.

Contributing isn’t limited to just code. We encourage you to contribute in the way that best fits your abilities, by writing tutorials, giving a demo at your local meetup, helping other users with their support questions, or revising our documentation.

For a more thorough introduction, [check out WP-CLI's guide to contributing](https://make.wordpress.org/cli/handbook/contributing/). This package follows those policy and guidelines.

### Reporting a bug

Think you’ve found a bug? We’d love for you to help us get it fixed.

Before you create a new issue, you should [search existing issues](https://github.com/schlessera/wp-cli-psysh/issues?q=label%3Abug%20) to see if there’s an existing resolution to it, or if it’s already been fixed in a newer version.

Once you’ve done a bit of searching and discovered there isn’t an open or fixed issue for your bug, please [create a new issue](https://github.com/schlessera/wp-cli-psysh/issues/new). Include as much detail as you can, and clear steps to reproduce if possible. For more guidance, [review our bug report documentation](https://make.wordpress.org/cli/handbook/bug-reports/).

### Creating a pull request

Want to contribute a new feature? Please first [open a new issue](https://github.com/schlessera/wp-cli-psysh/issues/new) to discuss whether the feature is a good fit for the project.

Once you've decided to commit the time to seeing your pull request through, [please follow our guidelines for creating a pull request](https://make.wordpress.org/cli/handbook/pull-requests/) to make sure it's a pleasant experience. See "[Setting up](https://make.wordpress.org/cli/handbook/pull-requests/#setting-up)" for details specific to working on this package locally.

## Support

Github issues aren't for general support questions, but there are other venues you can try: http://wp-cli.org/#support


*This README.md is generated dynamically from the project's codebase using `wp scaffold package-readme` ([doc](https://github.com/wp-cli/scaffold-package-command#wp-scaffold-package-readme)). To suggest changes, please submit a pull request against the corresponding part of the codebase.*

## How it Works

This package doesn't execute any PHP code, it simply [installs PsySh via Composer](https://github.com/schlessera/wp-cli-psysh/blob/83970ee52e6a0c3b2fac8b8165e23ce44a0f5a55/composer.json#L14-L15). The upstream `wp shell` command [looks for alternative shells](https://github.com/wp-cli/shell-command/blob/117147974eec7ad7eb43f3bf5006a48c79b2cd2e/src/Shell_Command.php#L47-L49) and loads one automatically if it exists.
