# @silvermine/video.js - A fork of [video.js][vjs]

This fork makes source setting synchronous in order to work around browser autoplay
policies. See [videojs/video.js#4765][src-setting-issue] for more information.

## Package release process notes

### Node and NPM versions

```bash
$ node -v
v6.10.3
$ npm -v
5.7.1
```

### Commands

```bash
nvm use 6.10.3
git fetch --all
git checkout silvermine_7.2.x
git status # make sure there are no uncommited changes
git reset origin/silvermine_7.2.x --hard
npm install
git status # make sure there are no uncommited changes
npm version "7.2.0-${NEW_BUILD_NUMBER}" -m "chore: Version bump: %s"
npm pack
npm publish "silvermine-video.js-7.2.0-${NEW_BUILD_NUMBER}.tgz"
```

[vjs]: https://github.com/videojs/video.js
[src-setting-issue]: https://github.com/videojs/video.js/issues/4765
