~~Def. | A logical operation is something that combines multiple statements to make a new statement.~~

Plus takes two numbers as an input and then outputs a new number.

A <b>logical operation</b> takes in one or more statement inputs and outputs a new statement.
- A binary logical operation takes in exactly two inputs. (AND, OR, XOR) ($\land \lor \oplus$)
- Tom Brady is a FB player $\land$ Valvo owns a shirt $\equiv$ T
- Tom Brady is a FB player $\land$ $2 + 2 = 5$  $\equiv$ F
- Tom Brady is a FB player $\lor$ $2 + 2 = 5$  $\equiv$ T

---

AND(P,Q){

 |P|Q|P$\land$Q|
 |---|---|---|
 |T|T|T|
 |T|F|F|
 |F|T|F|
 |F|F|F|

}

OR(P,Q){

 |P|Q|P$\lor$Q|
 |---|---|---|
 |T|T|T|
 |T|F|T|
 |F|T|T|
 |F|F|F|

}

XOR(P,Q){

 |P|Q|P$\oplus$Q|
 |---|---|---|
 |T|T|F|
 |T|F|T|
 |F|T|T|
 |F|F|F|

}

NOT(P) {

|P|~P|
|---|---|
|T|F|
|F|T|

}

IF-THEN(P,Q) { ^600c2f

|P|Q|P->Q|
|---|---|---|
|T|T|T|
|T|F|F|
|F|T|T|
|F|F|T|

}

### Does Order Matter for Logical Operations?
Ex. | Tom Brady plays football -> I have three arms $\equiv$ F $\equiv$ IF-THEN(T,F) $\equiv$ F
Ex. | I have three arms -> Tom Brady plays football $\equiv$ T $\equiv$ IF-THEN(F,T) $\equiv$ T

<b>Order does matter</b> [[Compound Statements#^547e9b]]

