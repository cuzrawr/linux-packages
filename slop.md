# Engineering principles

- Keep each package self-contained in its own directory.
- Prefer upstream release tarballs, verified checksums, and standard makepkg/Meson commands.
- Keep the upstream version in `pkgver` only; derive source URLs and directory names from it.
- Test build options before patches.
- Declare real dependencies, versioned replacements in `provides`, and matching `conflicts`.
- Preserve working image loaders, introspection, and package-manager cache hooks.
- Run upstream tests and check the built packages in a disposable builder. 
- Never install to the host.
- Document the reason for custom behavior and the ordinary update procedure. 
- Avoid wrapper frameworks, speculative options, and duplicated metadata.
