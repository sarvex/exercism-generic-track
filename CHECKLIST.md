Launch Checklist

## Step 1: Implement Exercises

- [ ] Implement at least 10 problems

See the [contributing guide](https://github.com/exercism/docs/blob/master/contributing-to-language-tracks/porting-an-exercise.md) for the details about the format of an exercise.

The short version is:

* a test suite
* an example solution, named with `example` (case-insensitive) in the filename
* a section in the "exercises" key of the config.json file with the slug, topics, and difficulty level.

The topics can be an empty list, and the difficulty level is from 1 to 10, and can default to 1 until we know more about the exercises.

```
"exercises": [
  {
    "slug": "hello-world" ,
    "difficulty": 1,
    "topics": []
  }
]
```

Problems are delivered to users in the same order that they are listed in this "exercises" array. Try to order them by increasing difficulty, but don't worry too much—it can always be adjusted later.

## Step 2: Prepare the Track for Launch

All of these steps are described in detail below.

- [ ] Define `test_pattern` in `config.json`
- [ ] Add a language icon or logo + attribution
- [ ] Write documentation in `docs/`
- [ ] Find track mentors

### test_pattern

The exercism.io website links to the exercise implementations, so it needs to know how to recognize the filename(s) for the test suite.

The `"test_pattern"` value in the `config.json` file should be a string that can be compiled as a regular expression, and which will match on the file or files that comprise the test suite of an exercise.

If the test filenames contain the word "test" (case insensitive) then the `"test_pattern"` key can be deleted.

### Language Icon and Attribution

We try to create a language icon that has the exercism colors, and is recognizably similar to the language icon. Sometimes this isn't possible due to copyright issues.

The Exercism colors are:

* `#D81D4E` (pink)
* `#212121` (charcoal)

The icon is used throughout the site in order to identify the language track, and to identify code that has been submitted to that track.

See http://exercism.io/languages for all the existing icons.

**Icon**

If image assets are not your strong suit, just find a reasonable image to start from, along with the information about the licensing, and we'll figure out the colorization thing (I've written some scripts to help me do this part).

The logo should be named `icon.png` and live under `img/` in this repository. If you know how, go ahead and make an SVG as well.

**Attribution**

The attribution goes in the `README.md` file.

If the icon we have based this on is not in the public domain, we need to provide information about license and provenance. If we require permission to use and/or change the icon, then we need to obtain that permission before we can use it.

### Documentation

For details about the various files and what they should contain, check out [writing language track documentation](https://github.com/exercism/docs/blob/master/maintaining-a-track/writing-documentation.md) in the [docs repository](https://github.com/exercism/docs).

### Find Track Mentors

Usually in order to see someone's solution you have to have submitted the exercise yourself. Track mentors can access all of the solutions in a given language. Track mentors can therefore help review solutions that people submit on the website in the beginning when few people have submitted solutions to exercises.

Ideally we should have a handful of people who are willing to check Exercism regularly to give people feedback, in order to start the track off on the right note.

The first track mentor needs to be added manually by @kytrinyx, but after that there's a section in the [account](http://exercism.io/account) where existing track mentors can invite new ones.

The most successful tracks are where **each submission receives feedback quickly**, preferably within the first 24 hours.

In addition, the most interesting and useful conversations start when reviewers do not direct users to do specific things, but rather ask questions challenging people to think about different aspects of their solution, or explore aspects of the language.

Referencing existing blog posts and style guides seems to work well when making specific recommendations.

## Prepare for Open Source Contributions

Once the track is live and active, it will often get new contributions.

- [ ] Read the maintainer documentation
- [ ] "Watch" the {{TRACK_ID}} repository
- [ ] Find a second maintainer
- [ ] Update the .github/PULL_REQUEST_TEMPLATE.md file

We've got a few years of experience maintaining language tracks on Exercism. Here's what we have learned:

- [Maintaining a Track](https://github.com/exercism/exercism.io/blob/master/docs/maintaining-a-track.md)
- [Reviewing a Pull Request](https://github.com/exercism/exercism.io/blob/master/docs/reviewing-a-pull-request.md)

There's more stuff in the [contributing guide](https://github.com/exercism/problem-specifications/blob/master/CONTRIBUTING.md), as well. We're working on turning that into better, more focused maintainer documentation.

## Step 3: Launch!

- [ ] Toggle `"active"` to `true` in `config.json`
- [ ] Mention it in the next "Behind the Scenes" newsletter (@kytrinyx)
- [ ] Add track mentors on the site (@kytrinyx)
- [ ] Add track maintainers to exercism/track-maintainers team (any organization owner)

