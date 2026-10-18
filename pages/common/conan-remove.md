# conan remove

> Remove Conan recipes and binary packages from the local cache or from a remote.
> See also: `conan upload`.
> More information: <https://docs.conan.io/2/reference/commands/remove.html>.

- Remove a recipe and all its binary packages from the local cache:

`conan remove {{package_name}}/{{version}}`

- Remove without asking for confirmation:

`conan remove {{package_name}}/{{version}} {{[-c|--confirm]}}`

- Remove only the binary packages that match a query, keeping the recipe:

`conan remove "{{package_name}}/{{version}}:*" {{[-p|--package-query]}} "{{os=Windows AND arch=x86_64}}"`

- Remove a recipe and its packages from a remote:

`conan remove {{package_name}}/{{version}} {{[-r|--remote]}} {{remote_name}}`

- Remove all revisions of a package except the latest one:

`conan remove "{{package_name}}/{{version}}#!latest"`

- Show what would be removed without removing anything:

`conan remove {{package_name}}/{{version}} --dry-run`
