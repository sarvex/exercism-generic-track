# Request a new Exercism language track

If there's a programming language that you would like Exercism to support, and which we don't
yet have a repository for, open a [new issue][new-issue] in this repository.

[new-issue]: https://github.com/exercism/request-new-language-track/issues/new

## How to bootstrap a new track

**Only owners of the organization can create new repositories.**

### One-time setup

1. Install [hub][].
1. Clone the [request-new-language-track][] repository.
1. Clone the [tools][] repository.
1. Follow the instructions in the [tools README][clone-tracks] to clone all the existing tracks.
1. Create a [saved reply][saved-replies] with the following checklist:

```
- [ ] Run bootstrap script
  `TRACK_ID=<id> LANGUAGE=<language> bin/bootstrap`
- [ ] Turn on [Travis CI][travis]
- [ ] If Windows-specific language, turn on [AppVeyor][appveyor]
- [ ] If Mac-specific language, turn on [Circle CI][circle]
  Add it as a Linux project, then switch it to OS X in _Project Settings -> Build Environment_
- [ ] Add as a submodule to [trackler][]
  `TRACK_ID=<id>; git submodule add https://github.com/exercism/x$TRACK_ID tracks/$TRACK_ID`
- [ ] Create [new team][new-team] for language
- [ ] Add bootstrapped repository to team **with write access**
- [ ] Invite requestor to team

[travis]: https://travis-ci.org/profile/exercism
[appveyor]: https://ci.appveyor.com/projects/new
[circle]: https://circleci.com/gh/organizations/exercism/settings#projects
[trackler]: https://github.com/exercism/trackler/tree/master/tracks
[new-team]: https://github.com/orgs/exercism/new-team
```

### Bootstrap a Track

Add the checklist as a reply to the issue request, then follow the checklist.

[saved-replies]: https://github.com/blog/2135-saved-replies
[request-new-language-track]: https://github.com/exercism/request-new-language-track
[tools]: https://github.com/exercism/tools
[clone-tracks]: https://github.com/exercism/tools#scripts
[hub]: http://github.com/github/hub
