# kokkos-mdspan
`build2` package for the [`kokkos mdspan implementation`](https://github.com/kokkos/mdspan) for C++20 and lower.

Note: This is the source code for the build2 package of the `kokkos/mdspan` C++ library, the actual library sources snapshot can be found in the ./upstream/ submodule.

## Usage

You can simply add this package as dependency to your project by specifying it in your `manifest`:

```
depends: kokkos-mdspan ^0.6.0
```

Then just pick the targets that you need:

```
import libs = mdspan%lib{mdspan}
```

Make sure to add the stable section of the cppget.org repository to your project's repositories.manifest to be able to fetch the package.

```
:
role: prerequisite
location: https://pkg.cppget.org/1/stable
# trust: ...
```

