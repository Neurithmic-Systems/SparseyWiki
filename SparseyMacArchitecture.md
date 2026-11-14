# The architecture of Sparsey's core (canonical) module

In Sparsey, the **mac** is the core processing module. It consists of $Q$ winner-take-all (WTA) **competitive modules** (CMs), each consisting of $K$ binary units ("cells").  Fig. 1a shows a mac with $Q=7$ CMs, each with $K=7$ cells. This architecture **structurally** [i.e., with **zero computational work (thus zero energy expenditure)**] enforces that during both: a) **learning**, i.e., storage of a memory (trace) of an input; and b) **inference**, i.e., retrieval (reactivation) of a previously stored memory trace, exactly $Q$ units will be activated, one per CM.  We call that **set** of $Q$ units a **code** and denote it with Greek letter, $&phi;$.  During a learning event, such as depicted in Fig. 1b, we say that the code is being stored. Fig. 1a,b shows an input level, in this case, an an 8x8 grid of binary input cells that is completely connected to the mac via a bottom-up ("U") matrix of synapses (weights) (blue lines). All weights initially have weight zero (i.e., are "naive"). 

![Tiny 2-level Sparsey model](tiny_2level_model.png)

