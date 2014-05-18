Tsdl — Thin bindings to SDL for OCaml
-------------------------------------------------------------------------------
Release %%VERSION%%

Tsdl is an OCaml library providing thin bindings to the cross-platform
SDL C library.

Tsdl depends on the [SDL 2.0.1][1] C library (or later) and
[ocaml-ctypes][2]. Tsdl is distributed under the BSD3 license.

[1]: http://www.libsdl.org/
[2]: https://github.com/ocamllabs/ocaml-ctypes

Home page: http://erratique.ch/software/tsdl  
Contact: Daniel Bünzli `<daniel.buenzl i@erratique.ch>`


## Installation

Tsdl needs the C library SDL 2.0.1 or later installed on your
system. Tsdl can be installed with `opam`:

    opam install tsdl

If you don't use `opam` consult the [`opam`](opam) file for
build instructions and a complete specification of the dependencies.


## Documentation

The documentation and API reference is automatically generated by
`ocamldoc` from the interfaces. It can be consulted [online][3] and
there is a generated version in the `doc` directory of the
distribution.

[3]: http://erratique.ch/software/tsdl/doc/


## Sample programs

Sample programs are located in the `test` directory of the
distribution. They can be built with:

    ocamlbuild -use-ocamlfind tests.otarget

The resulting binaries are in `_build/test` :

- `test.native`, tests the bindings, the executable should exit 
   with 0.
- `sdlevents.native`, traces SDL events.
- `min.native` a minimal SDL example.
