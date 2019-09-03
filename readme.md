# Repro

```
yarn
cd android
./gradlew assembleRelease --stacktrace
```

Now check content of `./android/app/build/generated/sourcemaps/react/release/index.android.bundle.map`

Expected:
```
"x_facebook_sources":
```
in the source map to be filled.

Actual:
```
"x_facebook_sources":[null,null,null ....
```
All values are `null`.