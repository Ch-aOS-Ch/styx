# styx
Ch-aOS plugin registry

## What is it?

This is a place where to install your Ch-aOS plugins, of all shapes, sizes and types

## How to install?

Just do a `chaos styx install {name of your plugin}` and done

## How to publish?

1. Create a branch with your package name.
2. insert your package with it's required metadata (about, git repo, version of the package and name) inside of the registry.yaml file as another item to the dictionary, it's name should be the key to your metadata dict.
3. profit.

> [!WARNING]
>
> for Ch-aOS to be able to install your package, it must be inside of your releases as a .whl file, Ch-aOS will reject everything else.

> [!WARNING]
>
> Ch-aOS plugins should be as self contained as possible. Styx is dumb by design, it does not manage versions or even dependencies.
