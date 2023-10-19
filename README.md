# swift-code-coverage
Code Coverage for the Swift AutoDiff unit tests

Generated with this process:

1. build-script ... --dry-run
2. build-script ...
3. Modify CMakeCache.txt: add profiling flags for both CMAKE_CXX_FLAGS and CMAKE_SWIFT_FLAGS
4. Redo the process for building swift-* folder from the build-script
5. Run AutoDiff test cases with test-script
6. llvm tools to merge and show profdata
