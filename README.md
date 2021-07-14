# @silvermine/video.js - A fork of [video.js][vjs]

This fork makes source setting synchronous in order to work around browser autoplay
policies. See [videojs/video.js#4765][src-setting-issue] for more information.

## Package release process notes

### Node and NPM versions

```bash
$ node -v
v12.22.1
$ npm -v
6.14.2
```

### Commands

```bash
nvm use 12.22.1
git fetch --all
git checkout silvermine_7.19.x
git status # make sure there are no uncommitted changes
git reset origin/silvermine_7.19.x --hard
npm install
git status # make sure there are no uncommitted changes
npm version "7.19.0-${NEW_BUILD_NUMBER}" -m "chore: Version bump: %s"
npm pack
npm publish "silvermine-video.js-7.19.0-${NEW_BUILD_NUMBER}.tgz"
```

[vjs]: https://github.com/videojs/video.js

[src-setting-issue]: https://github.com/videojs/video.js/issues/4765
