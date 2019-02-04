# Reasonml/OCaml glossary

Greetings, wanderer. Reason and OCaml ecosystem are now growing extremely fast and may want to go aboard this train. But if you're coming from another ecosystem, say .NET of Java or JS (though it would be easier for frontend folks, because Reason ecosystem tries to be webstack-compatible), you may find this esy, dune, bucklescript, jsoo and whole bunch of other stuff pretty confusing. So I dared to cobble up a glossary of terms and tools for you to be in the context.

## Need to know

* Reason and OCaml are interchangeable in a sence that you can convert Reason to OCaml and visa-versa. So if you see OCaml lib that suits your needs, but you're writing Reason - you can use it. Though beware that this lib may not be compatible with web platform.  Note that libraries written is Reason tend to be more compatible.

## Tools

* [**Bucklescript**](https://bucklescript.github.io/) - build system to build javascript from Reason/OCaml. It's simple, you can install it from npm and it produces kinda readable output. Considered as modern way to use Reason stack for frontend development. Packages for bucklescript usually use `bs-` prefix (e.g. `bs-fetch` is Reason/OCaml bindings to browsers `fetch` API)
* [**JSOO - Js of OCaml**](https://github.com/ocsigen/js_of_ocaml) - another OCaml->Js transpiler. Focuses more on producing perfomant code. Read [Bucklescript to JSOO comparison](https://bucklescript.github.io/docs/en/comparison-to-jsoo) for more details
* [**Esy**](https://esy.sh/) - npm-like (more yarn-like actually) package manager for both native and js Reason/OCaml. It can work with both npm and opam repositories.
* [**Pesy**](https://github.com/esy/pesy) - ?
* [**Opam**](https://opam.ocaml.org/) - default package manager for native Reason/OCaml
* [**Dune**](https://github.com/ocaml/dune) - build system for native Reason/OCaml
* [**Refmt**](https://github.com/polydawn/refmt) - ?
* [**Merlin**](https://github.com/ocaml/merlin) - library for editor support
* [**Odoc**](https://www.reason-association.org/projects/odoc/) - HTML documentation generator for Reason/OCaml

## Terms

* `ppx` - extensions point for language. E.g. `let%bind` from [ppx_let](https://github.com/janestreet/ppx_let) allows you to not to match on option manually. Kinda like [F# builders](https://docs.microsoft.com/en-us/dotnet/fsharp/language-reference/computation-expressions)
* `FFI` - foreign function interface, which means a way/ a syntax to use for interoperability with other languages like C or JS. It's not actually specific to Reason/OCaml, but they have a uniform way to declare such ffi.
