* It's a **monad** because it is a parameterized type (**Optional<T>**) that:
  * Implements a bind operation **flatMat()**
  * Implements a unit function **of()**
  * Follows three laws: _left identity_, _right identity_ and _associativity_