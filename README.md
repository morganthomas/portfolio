# Morgan Thomas project portfolio

Here are some selected open source code bases where I am a primary contributor.

## Zero knowledge cryptography

### Valida

I am technical lead and at times an individual contributor on [the Valida VM by Lita](https://github.com/lita-xyz/valida-vm) since mid-2023, as well as [the Valida tooolchain by Lita](https://github.com/lita-xyz/valida-releases), which consists of the Valida VM (open-source) and the Valida compiler toolchain (closed-source).

### Open Specification Language (OSL) compiler

I am the primary author of the Open Specification Language (OSL) and [its Haskell compiler](https://github.com/Polytopoi/osl).
This is a high-level specification language designed to be compiled efficiently to arithmetic circuits. 

### Haskell FRI proofs

I am a primary author of [Orbis haskell-fri-proofs](https://github.com/Orbis-Tertius/haskell-fri-proofs).This codebase contains an
implementation of [FRI (Fast Reed-Solomon IOP of Proximity)](https://www.semanticscholar.org/paper/Fast-Reed-Solomon-Interactive-Oracle-Proofs-of-Ben-Sasson-Bentov/2415603b4e8799f575b788706be21862c055e25b), and a partial implementation of the PLONK IOP, in Haskell.

### TinyRAM emulator

I am a primary author of [the Orbis TinyRAM emulator](https://github.com/Orbis-Tertius/tinyram), an emulator for the
TinyRAM zkVM architecture written in Haskell.

## Haskell frontend development

### Shpadoinkle

I am a major contributor to [Shpadoinkle](https://shpadoinkle.org/), the Haskell UI framework. I am responsible for the concept of Shpadoinkle continuations, which is how Shpadoinkle allows for concurrent event handlers interacting with view models without race conditions. I am also responsible for Shpadoinkle's mechanisms for streaming data, lazy loading tables, and lazily populated tables.

**Source:** https://gitlab.com/fresheyeball/Shpadoinkle

### servant-client-js

This is an alternative to [`servant-client`](https://github.com/haskell-servant/servant) for use in web browsers. Servant is a Haskell framework for building APIs. `servant-client` is a part of Servant which deals with automatically creating functions to call Servant APIs. `servant-client` supports being used in web browsers, but in this context it does not support streaming HTTP responses, because under the hood it uses `XMLHttpRequest`, which does not support streaming responses. Therefore I made `servant-client-js`, which uses the Fetch API under the hood and supports streaming HTTP responses. I did this by myself. This library is a dependency of Shpadoinkle.

**Source:** https://github.com/morganthomas/servant-client-js
