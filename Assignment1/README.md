- ## General boundary
The general boundary G, with respect to hypothesis space H and training
data D, is the set of maximally general members of H consistent with D.<br>
![image](https://user-images.githubusercontent.com/64849889/141343101-4d2d2b51-c818-4cb7-90c6-9ba54ab0ef7f.png)

- ## Specific boundary
The specific boundary S, with respect to hypothesis space H and training
data D, is the set of minimally general (i.e., maximally specific) members of H
consistent with D.
![image](https://user-images.githubusercontent.com/64849889/141343196-c04aba58-7945-46b8-9286-7280eb1418dc.png)

- ## Version space representation theorem
Let X be an arbitrary set of instances and let H be a set of boolean-valued hypotheses defined over X. Let c : X + {O, 1} be an arbitrary target concept defined over X and let D be an arbitrary set of training examples {<x, c(x)>}. For all X, H, c, and D such that S and G are well defined, 

![image](https://user-images.githubusercontent.com/64849889/141342831-5dc12c05-0cc7-4e7d-b923-3a6fcabb757f.png)

Proof: To prove the theorem it suffices to show that<br>
(1) every h satisfying the righthand side of the above expression is in VS<sub>H,D</sub>.<br>
(2) every member of  VS<sub>H,D</sub> satisfies the right-hand side of the expression.<br>

To show (1) let g be an arbitrary member of G, s be an arbitrary member of S, and h be an arbitrary member of H, such that g>=<sub>g</sub> h>=gs. Then by the definition of S, s must be satisfied by all positive examples in D. Because h>=<sub>g</sub> s, h must also be satisfied by all positive examples in D. Similarly, by the definition of G, g cannot be satisfied by any negative example in D, and because g>=<sub>g</sub> h, h cannot be satisfied by any negative example in D. Because h is satisfied by all positive examples in D and by no negative examples in D, h is consistent with D, and therefore h is a member of VS<sub>H,D</sub>.
This proves step (1). The argument for (2) is a bit more complex. It can be proven by assuming some h in  VSH,D that does not satisfy the right-hand side of the expression, then showing that this leads to an inconsistency.
