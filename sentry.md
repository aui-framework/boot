# Sentry (native)

```cmake
auib_import(sentry https://github.com/Alex2772/sentry-native-no-ca-check
        FORCE_STATIC
        VERSION e1ba734
        CMAKE_ARGS -DSENTRY_TRANSPORT=curl -DSENTRY_BACKEND=inproc -DSENTRY_BUILD_TESTS=OFF -DSENTRY_BUILD_EXAMPLES=OFF
        REQUIRES CURL OpenSSL ZLIB)
aui_link(YOUR_APP PUBLIC sentry::sentry)
```

or

```cmake
auib_import(sentry https://github.com/getsentry/sentry-native
            CMAKE_ARGS -DSENTRY_BACKEND=crashpad)
aui_link(YOUR_APP PUBLIC sentry::sentry)
```

