# conan upload

> Upload Conan recipes and binary packages to a remote.
> See also: `conan remove`.
> More information: <https://docs.conan.io/2/reference/commands/upload.html>.

- Upload a recipe and all its binary packages to a remote:

`conan upload {{package_name}}/{{version}} {{[-r|--remote]}} {{remote_name}}`

- Upload without asking for confirmation:

`conan upload {{package_name}}/{{version}} {{[-r|--remote]}} {{remote_name}} {{[-c|--confirm]}}`

- Upload only the recipe, not the binary packages:

`conan upload {{package_name}}/{{version}} {{[-r|--remote]}} {{remote_name}} --only-recipe`

- Upload only the binary packages that match a query:

`conan upload {{package_name}}/{{version}} {{[-r|--remote]}} {{remote_name}} {{[-p|--package-query]}} "{{os=Linux AND arch=x86_64}}"`

- Check the integrity of the packages with their manifests before uploading:

`conan upload {{package_name}}/{{version}} {{[-r|--remote]}} {{remote_name}} --check`

- Upload even if the same revision already exists on the remote:

`conan upload {{package_name}}/{{version}} {{[-r|--remote]}} {{remote_name}} --force`
