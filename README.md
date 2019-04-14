# FOL_Parser
First Order Logic Parser


Test Cases :
Bill has at most one sister.
∀ x, y ( SisterOf(x, Bill) ∧ SisterOf(y, Bill) ⇒ x = y )
fol(PT,[forall,x,y,"(",s,"(",x,y,")",and,s,"(",x,y,")",implies,x,=,y,")"],[]).

Every student loves some student.
∀ x ( Student(x) ⇒ ∃ y ( Student(y) ∧ Loves(x,y) )).
fol(PT,[forall,x,"(",s,"(",x,")",implies,exists,y,"(",f,"(",y,")",and,l,"(",x,y,")",")",")"],[]).


There exists a student.
∃ x Student(x).
fol(PT,[exists,x,"(",f,"(",x,")",")"],[]).


For all x ,y (f(x) implies g(y)).
fol(PT,[forall,x,y,"(",f,"(",x,")",implies,g,"(",y,")",")"],[]).
