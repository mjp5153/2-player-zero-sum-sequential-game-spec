# 2-player zero-sum sequential game specification JSON-schema

This project defines a standard way of representing 2-player zero-sum sequential games, for use with
applicable game theory algorithms.  

Included are two examples, including a simple "Even or odd" game, as well as [Kuhn poker](https://en.wikipedia.org/wiki/Kuhn_poker).

The JSON-scema validates the structure, but one additional piece of validation is necessary: for any action specified, the
value must match the name of an existing state.  If not, the game contains a broken link.  This is
a known issue in the schema that should be correct.  For now, make sure to validate this manually in 
any software that utilizes this specification.  

Copyright 2021 Mike Peters.  Source code available under Apache License, Version 2.0.