### Collectors

* Accumulate elements into a mutable result container (Collection, String, ...)
* Consists of three things:
  - A **supplier** of an initial value
  - An **accumulator** which adds to the initial value
  - A **combiner** which combines two results into one
* Use **collect(supplier,accumulator,combiner)** or **collect(Collector)**
