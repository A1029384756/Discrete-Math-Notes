[[Logical Operations]]
Two expressions are equivalent if for every possible way to input truth values into the variables, the statements have the same truth value.

>We can check this with a truth table.

Claim: ~(P$\land$Q)$\equiv$~P$\land$~Q

|P|Q|~P|~Q|P$\land$Q|~(P$\land$Q)|~P$\land$~Q|
|---|---|---|---|---|---|---|
|T|T|F|F|F|F|F|
|T|F|F|T|F|<b>T</b>|<b>F</b>|
|F|T|T|F|F|<b>T</b>|<b>F</b>|
|F|F|T|T|F|T|T|
This claim is false.
> If the truth tables differ between any two logical statements, they are not equivalent.

Claim: ~(P$\land$Q)$\equiv$P$\oplus$Q

|P|Q|P$\land$Q|~(P$\land$Q)|P$\oplus$Q|
|---|---|---|---|---|
|T|T|T|F|F|
|T|F|F|T|T|
|F|T|F|T|T|
|F|F|F|<b>T</b>|<b>F</b>|
This claim is false.

Claim: ~(P$\land$Q)$\equiv$~P$\lor$~Q

|P|Q|~P|~Q|~(P$\land$Q)|~P$\lor$~Q|
|---|---|---|---|---|---|
|T|T|F|F|F|F|
|T|F|F|T|T|T|
|F|T|T|F|T|T|
|F|F|T|T|T|T|
This claim is true.
> Since the two expressions yield the same output for any input, they are logically equivalent. [[Logical Equivalence]]

---
