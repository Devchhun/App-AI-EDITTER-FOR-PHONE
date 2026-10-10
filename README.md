# Creative AI Editor for Phone

Android video editor built with React, Capacitor and native Android media tools.

## Development

```sh
npm ci
npm run typecheck
npm run apk
```

The APK is written to `dist-apk/`.

## Publishing an update

Update `version` in `package.json`, `versionCode` and `versionName` in
`android/app/build.gradle`, commit the change, then push a matching version tag:

```sh
git tag v0.5.3
git push origin main --tags
```

GitHub Actions builds the APK and attaches it to a GitHub Release. The phone
app checks the latest release from `Devchhun/App-AI-EDITTER-FOR-PHONE`.
