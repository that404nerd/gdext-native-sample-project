## To build:
```bash
# Create build/ and build the project first
mkdir build && cd build
cmake -B gdext-native-build -DCMAKE_BUILD_TYPE=Debug -DCMAKE_EXPORT_COMPILE_COMMANDS=1 -DCMAKE_INSTALL_PREFIX=gdext-native-install gdext-native ..

# Install
cmake --build gdext-native-build -j8
cmake --install gdext-native-build
```

- Link the `compile_commands.json` to the root of the project:
`ln -s build/gdext-native-build/compile_commands.json .`