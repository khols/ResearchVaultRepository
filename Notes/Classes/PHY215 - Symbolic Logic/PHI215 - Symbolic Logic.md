# Sept. 18th, 2025
## John Searle & AGI
### “Chinese” Room Experiment
- If you send symbols into a room and inside the room is a book of all natural language rules in symbolic form and a person, if the symbols are sent in translated and sent out, do the person and the room actually understand what is being translated. 
## Logical Language Parts
### Syntax
- First order logic
	-  $L_{1}=\{ v,\&,\to,\sim,(,),P,Q,\dots \}$
- Second order
	- $L_{2}=\{ L_{1},a,b,c,d,e,\dots, P\_,Q\_\ \_,R\_\ \_\ \_, \dots \}$
	- Arity → the number of arguments or operands taken by a function
		- $B_j$ : John is bald
	- Domain must be defined
		- Often is → Everything in the world
		- $_j$ = John Beverly
		- $B\_$ = is bald
### Semantics
- Truth tables for v,&,→,~
### Proof Theory
- Rules for preserving truth from premises to conclusion
	- I.e. validity
## Logic Recipes
- If
- Only if
- Iff (if and only if)
- And
- Or
- Neither nor
- Not both
- Not
### Bi-conditional
- (P→Q) & (Q→P) is the same as (P ←→ Q)
- It means “if and only if”
	- Sometimes denoted as “iff”
### Unless
- It can be described as either “if not” or “or”
	- ~(Q→P)
	- Q v P
### Neither Nor
- Neither P nor Q
	- ~(P v Q)
- Not both P & Q
	- ~(P & Q)
## Examples
- John and Tom are cousins.
	- Wrong answers:
		- (J & T) & C
		- P = John is cousin with Tom. Q = Tom is cousin with John. (P & Q)
	- New try:
		- Domain: everything in the world
		- $C\_ \ \_$ = is cousins (more properly: cousin of)
		- $_j$ = John
		- $_t$ = Tom
		- $C_{jt}$ 

# Sept 23rd, 2025
## Proof Theory
- Validity
- Rules of inference
- Soundness
- Completeness
- Longer “sentences” can be instantiated using meta-variables
- Conditional elimination (CEL) / Modus Ponens (MP)
	- Q → R
	- Q
	- Therefore R
- Conjunction elimination (CE)
	- Q & R
	- Therefore Q
- Conditional induction (CI)
	- Q
	- R
	- Therefore Q & R
- Disjunction induction (DI)
	- Q
	- Therefore Q v R
- Disjunction elimination (DE)
	- Q v R
	- ~ Q
	- Therefore R
- Double Negation elimination (NE / DNE)
	- ~~ Q
	- Therefore Q
- Negation induction (NI)
	- Q
	- Therefore ~~ Q
- Modus Tollens (MT)
	- P → R
	- ~R
	- ∴ ~P
- Bi-conditional Elimination
	- Q ←→ X
	- (Q→X) & (X→Q)
- Bi-conditional Induction
	- Q ←→ X

### Questions
1) .
	1. P & Q 
	2. SHOW P
	3.  P (1, CE)
2) .
	1) P & S 
	2) (R & S) → ~T
	3) R
	4) SHOW ~T
	5) S (1, CE)
	6) (R & S) (3,5, CI)
	7) ∴ ~T (2,6 CEL)
3) .
	1) P & S
	2) ~T
	3) R
	4) SHOW R v ((P & Q) → X)
	5) R v ((P&Q) → X) (3, DI)
4) .
	1) (P v Q) → ~R
	2) P & T
	3) R v ~S
	4) U → S
	5) SHOW ~U
	6) P (2, CE)
	7) P v Q (6, DI)
	8) ~ R (1,7 CEL)
	9) ~ S (3,8 DE)
	10) ~ U (4,9 MT)
5) .
	1) A → B
	2) (A → B) → (B→A)
	3) (A ↔ B) → A
	4) SHOW A & B
	5) (B→ A) (CEL, 1,2)
	6) (A→B) & (B→A) (1,5 CI)
	7) A↔B (6, BI)
	8) A (3,7 CEL)
	9) B (1,8 CEL)
	10) A & B (8,9 CI)
6) . Not sure if this one is right
	1) ~A & B
	2) (C v B) → (~D → A)
	3) ~D ↔ E 
	4) SHOW ~E
	5) ~A (CE, 1)
	6) B (CE, 1)
	7) (~ D → A) (CEL, 1,2)
	8) (~D → E) & (E → ~D) (BE, 3)
	9) (E → ~D) (8, CE)
	10) D (MT, 5,7)
	11) ~E (MT, 8,9)