# Exercism {{LANGUAGE}} Track

![build status](https://travis-ci.org/exercism/xslug.svg?branch=master)

Exercism exercises in {{LANGUAGE}}.

## Setup

The simplest way to install {{LANGUAGE}} is ...

## Contributing

Thank you so much for contributing! :tada:

Please start by reading how to [get involved in a track](https://github.com/exercism/exercism.io/blob/master/docs/getting-involved-in-a-track.md). Comprehensive details on contributing can be found [here](https://github.com/exercism/x-common/blob/master/CONTRIBUTING.md). Be sure to read the Exercism [Code of Conduct](https://github.com/exercism/exercism.io/blob/master/CODE_OF_CONDUCT.md).

We welcome pull requests that provide fixes and improvements to existing exercises. If you're unsure, then go ahead and open a GitHub issue, and we'll discuss the change.

Please keep the following in mind:

- Pull requests should be focused on a single exercise, issue, or change.

- We welcome changes to code style, and wording. Please open a separate PR for these changes if possible.

- Please open an issue before creating a PR that makes significant (breaking) changes to an existing exercise or makes changes across many exercises. It is best to discuss these changes before doing the work. Discussions related to exercises that are not track specific can be found in [exercism/discussions](https://github.com/exercism/discussions/issues).

- Follow the coding standards for {{LANGUAGE}}. (If there is a formatter for the track's language, add instructions for using it here.)

- Watch out for trailing spaces, extra blank lines, and spaces in blank lines.

- Each exercise must stand on its own. Do not reference files outside the exercise directory. They will not be included when the user fetches the exercise.

- Exercises should use only the {{LANGUAGE}} core libraries.

- Please do not add a README or README.md file to the exercise directory. The READMEs are constructed using shared metadata, which lives in the
[exercism/x-common](https://github.com/exercism/x-common) repository. Further explanation can be found in [fixing-exercise-readmes](https://github.com/exercism/exercism.io/blob/master/docs/fixing-exercise-readmes.md)

- Each exercise should have a test suite, an example solution, a template file for the real implementation and ... (anything else that needs to go with each exercise for this track). The CI build expects files to be named using the following convention: (describe the {{LANGUAGE}} convention for naming the various files that make up an exercise).

- Make sure everything is good to go by running all tests with ... (explain how to run the full build locally, commonly `bin/build.sh`).

- Please do not commit any configuration files or directories inside the exercise other than ...

- Test files should use the following format:

```
# include the body of an example test
```

- All the tests for {{LANGUAGE}} exercises can be run from the top level of the repo with ... Please run this command before submitting your PR.

- If you are submitting a new exercise, be sure to add it to the appropriate place in the `config.json` file. Also, please run `bin/fetch-configlet && bin/configlet` to ensure the exercise is configured correctly.
