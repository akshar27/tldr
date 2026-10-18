# conan new

> Create a new Conan recipe and example source files from a template.
> Built-in templates include `basic`, `cmake_lib`, `cmake_exe`, `header_lib`, `meson_lib`, and `autotools_lib`.
> More information: <https://docs.conan.io/2/reference/commands/new.html>.

- Create a simple recipe with example code and helpful comments:

`conan new basic`

- Create a CMake library recipe with a given name and version:

`conan new cmake_lib {{[-d|--define]}} name={{package_name}} {{[-d|--define]}} version={{1.0}}`

- Create a CMake executable recipe:

`conan new cmake_exe {{[-d|--define]}} name={{package_name}} {{[-d|--define]}} version={{1.0}}`

- Create a CMake library recipe that depends on another package:

`conan new cmake_lib {{[-d|--define]}} name={{package_name}} {{[-d|--define]}} version={{1.0}} {{[-d|--define]}} requires={{dependency/version}}`

- Create the recipe files in a specific directory:

`conan new cmake_lib {{[-d|--define]}} name={{package_name}} {{[-d|--define]}} version={{1.0}} {{[-o|--output]}} {{path/to/directory}}`

- Overwrite files that already exist:

`conan new cmake_lib {{[-d|--define]}} name={{package_name}} {{[-d|--define]}} version={{1.0}} {{[-f|--force]}}`
