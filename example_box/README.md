# Vagrant OCI Example Box

Vagrant providers each require a custom provider-specific box format.
This folder shows the example contents of a box for the `oci` provider.

To build the box:

```
$ tar cvzf oci.box ./metadata.json ./Vagrantfile
```

This box works by using Vagrant's built-in Vagrantfile merging to setup
defaults for OCI. These defaults can easily be overwritten by higher-level
Vagrantfiles (such as project root Vagrantfiles).
