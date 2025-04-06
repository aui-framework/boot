# Boost

```cmake
auib_import(Boost https://github.com/boostorg/boost/releases/download/boost-1.84.0/boost-1.84.0.tar.xz
    ARCHIVE
    CMAKE_ARGS -DBOOST_ENABLE_CMAKE=ON
)

aui_link(${PROJECT_NAME} PRIVATE Boost::boost)
```
