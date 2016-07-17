# A Colored Petri Net Erlang/OTP library [![Build Status](https://travis-ci.org/joergen7/gen_pnet.svg?branch=master)](https://travis-ci.org/joergen7/gen_pnet)

**[gen_pnet documentation](http://cuneiform-lang.org/man/gen_pnet/)**

Some applications exhibit behavioral patterns that lend themselves to Petri Nets. The major advantage of modeling applications with Petri Nets is that they provide a natural view on the concurrent behavior of an application. This is achieved by making explicit the preconditions for an operation to be carried out while leaving implicit how and when an operation is triggered and what other operations might run in parallel.

This OTP library is a framework for programming with Petri Nets. It implements a very general form of Petri Nets: Colored Petri Nets (CPN). I.e., tokens may not only be markers but can be any conceivable data structure. Furthermore, a place can hold any number of tokens not just one.

While many simulation libraries only mimic the concurrent behavior of Petri Nets, the `gen_pnet' library allows the definition of Nets with an arbitrary number of transitions competing for a place's tokens neither imposing order in the form of an orverarching loop nor otherwise constraining parallelism.

