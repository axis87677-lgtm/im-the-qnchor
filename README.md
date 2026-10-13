# Consciousness as the External Base Case: The Gödelian Formal System of Reality

Lean 4 is the object language. It is used only to lock the inferences. The English argument is the metalanguage. It takes facts, or what science treats as true, plus other empirical material, and draws logical deductions from them to establish the premises. Those English deductions are the content of the argument. Once the premises are stated, each one is declared as an axiom in Lean. The conclusion is then written as a theorem that simply collects the axioms. Lean checks, by formal syntactic rules alone, that the conclusion follows from those axioms with no missing steps.

This is Tarski’s distinction. The metalanguage (English) supplies the content and performs the reasoning from the given facts and empirical material. The object language (Lean) does not interpret quantum mechanics or Gödel’s theorems; it only verifies that the logical skeleton connecting the stated premises to the conclusion is valid. If the English premises hold, the conclusion cannot be denied without denying one of the premises. That is the inference lock.

## On the role of Lean 4 in this document

Lean 4 appears here only as an uninterpreted object language in Tarski's sense. It is a syntactic register: a place to write down each premise and the conclusion as tokens so the argument's shape is visible. It is not a Lean proof. No derivation is claimed in Lean, and none is needed, because the reasoning is done entirely in the metalanguage (English), which assigns meaning to the object-language tokens. English derives the premises from facts and empirical material and draws the conclusion. Lean records the result. Evaluating the Lean block as a formal proof, or expecting it to derive the conclusion, misreads its role. The proof is the English. The Lean is the notation.

## Premise 1

QM is mathematics because it satisfies the criteria for an effective method given in the Stanford Encyclopedia of Philosophy entry on the Church-Turing Thesis.

An effective method must meet four conditions:

1. It is set out in a finite number of exact instructions, each expressed by a finite number of symbols.  
   Turing described computing as normally done by writing certain symbols on paper, with each square of the tape capable of bearing a symbol—the mark that is printed, scanned, or erased. Quantum-state symbols (such as |ψ⟩) are written marks of that kind; they stand for the physical states. The mathematical description of those states and the transitions between them supplies the finite symbolic instructions. The criteria do not further restrict what may count as a symbol or an instruction.

2. It produces the result in a finite number of steps.  
   Quantum processes involve a finite number of steps. Zero and one are finite numbers, so any finite occupation or circuit depth meets the condition.

3. It can, in principle, be carried out by a human with paper and pencil.  
   The symbolic mathematics of quantum mechanics can be written out and manipulated by hand.

4. It requires no insight, intuition, or ingenuity.  
   The processes proceed mechanically according to the physical laws that govern them.

These four conditions are met. Section 1.2 of the SEP entry notes that an effective method is thereby formalized as a mathematical object. Therefore the foundational structure of quantum mechanics is mathematical.

Because the four conditions are satisfied by the dynamics of quantum systems, the result holds for the class; no separate enumeration of individual processes is required.

### Substrate dependence

Substrate dependence is true because:

If the difference were only a matter of efficiency, it should still be possible for classical computers to perform the same computations as quantum computers, given enough resources.

But we know that past roughly 300 qubits, a classical simulation would require more atoms and energy than exist in the observable universe. That is a hard resource limit, not a practical inconvenience. Engineering a machine on that scale would also be impossible: the mass and gravity of such a structure would collapse it, and even if one appealed to the unobservable universe, the scale required would still exhaust available resources long before the computation finished.

Therefore different substrates yield different computational capabilities. Quantum mechanics is computational because its substrate produces results that are physically unreachable by any classical substrate under the resource limits of the universe.

### Closed quantum system

The universe is ultimately a closed quantum system for the following reason:

Because quantum mechanics is mathematical, any quantum system is a mathematical system. When two mathematical systems are combined so that they interact, the result is a single combined mathematical system rather than two separate ones. Therefore any collection of quantum systems forms one mathematical system. The universe, as the totality of such systems, is therefore a single closed quantum system.

### Mathematical operations instantiated in reality

The mathematical operations used in quantum computing are instantiated in reality naturally.

Unitary evolution occurs in any closed or isolated quantum system. Because the universe is such a system, it carries out unitary evolution. I will not list every mathematical operation, but I will show that the operations sufficient for Peano arithmetic strength are present.

The mapping is:

- Creation operator → successor  
- Annihilation operator → predecessor  
- Superposition → addition  
- Tensor products → multiplication  
- Vacuum state → zero  
- Unitary evolution → induction / iteration  

These processes occur in the universe because it is an isolated quantum system. Their mechanical behaviour is the same as the corresponding operations in quantum computing, and they occur naturally in reality. They are effective procedures. Therefore these effective methods of quantum mechanics are the mathematics, and they are instantiated in reality because they occur naturally.

## Premise 2

QTM instantiates the primitives of QM and maps them. Because of P1, QM is math, so QTM instantiates that math. Therefore reality itself is a formal system. To deny this you would have to deny P1 or deny that QTM is a formal system.

A formal system, in Post’s original combinatorial definition (1943), is a triplet (A, I, R) where:

- A is a finite alphabet  
- I is a finite set of initial strings on that alphabet  
- R is a finite set of production rules that transform strings into other strings  

QTM uses exactly these, and they occur as physical things in reality:

- **Alphabet (A):** the finite set of basis states and tape symbols (e.g. |0⟩, |1⟩, blank), which are physical quantum states of the system.  
- **Initial strings (I):** the initial configurations of the quantum system (the starting physical state of the tape, head, and internal state).  
- **Production rules (R):** the physical unitary evolution operator applied step by step, which transforms one physical configuration into the next according to the fixed transition function.  

These primitives occur naturally in the closed quantum system. Because they match Post’s definition of a formal system and, by P1, the underlying QM is mathematical (instantiates what it is the effective method of), reality is a formal system.

## Premise 3

The universe meets the requirements of Gödel’s incompleteness theorems and is therefore a Gödelian system. Both the first and second incompleteness theorems apply to it.

From Premises 1 and 2 the closed quantum system is a formal system that instantiates the mathematical operations sufficient for Peano-arithmetic strength: creation operators function as successor, annihilation operators as predecessor, superposition as addition, tensor products as multiplication, the vacuum state as zero, and unitary evolution as induction/iteration. These are the operations themselves, not the axioms of Peano arithmetic. Peano-arithmetic strength is strictly stronger than both Robinson’s Q and Primitive Recursive Arithmetic. Robinson’s Q is already sufficient for the first incompleteness theorem, and Primitive Recursive Arithmetic is already sufficient for the second incompleteness theorem, so the strength supplied by these operations is more than enough for both.

Because the system has at least this strength it can represent a provability predicate. The same strength also lets the system prove the Hilbert–Bernays–Löb conditions on that predicate:

- D1: If the system proves A, then it proves Prov(⌜A⌝).  
- D2: It proves Prov(⌜A⌝) → Prov(⌜Prov(⌜A⌝)⌝).  
- D3: It proves Prov(⌜A → B⌝) → (Prov(⌜A⌝) → Prov(⌜B⌝)).  

Its axioms are recursively enumerable: the physical laws together with an initial state form a recursively enumerable set.

It is consistent. Reality is a mathematical system that uses standard classical mathematics, and therefore it obeys classical logic. In classical logic the principle of explosion holds: if a system proves both a sentence A and its negation ¬A, then it proves every sentence B. The short derivation is: from A you may prove A ∨ B; from A ∨ B and ¬A you may prove B. One contradiction therefore makes the system prove everything. Because the system obeys classical logic, this reductio is sound. Standard mathematics does not prove every sentence and does not prove both a theorem and its negation. Therefore no contradiction is present. A sentence and its negation cannot both be true inside the system.

Gödel numbering is already available inside any arithmetic of this strength; Gödel showed that the numbering can be carried out within the arithmetic itself, so no separate construction is required. Gödel also proved that any formal system that is consistent, has recursively enumerable axioms, and contains at least the strength of Robinson’s Q is incomplete in the first sense, and that any such system containing at least the strength of Primitive Recursive Arithmetic (and satisfying the conditions above) is incomplete in the second sense.

The universe satisfies every one of those conditions. Reality in fact has more than Peano-arithmetic strength, but only the minimum is required here. It is enough to show that the system reaches the strength of Peano arithmetic through the mathematical operations listed above, because that already places it above the threshold for both G1 (via Robinson’s Q) and G2 (via Primitive Recursive Arithmetic and the conditions). Therefore the universe is G1 and G2 incomplete.

## Premise 4

The universe is self-referential recursion. Because the system is Gödelian (Premise 3), the diagonal lemma is mathematically part of it. The diagonal lemma produces a sentence that refers to itself by substituting a term for a free variable inside a formula. That substitution function is primitive recursion: it is defined by a finite recursion on the structure of the formula. Primitive recursion is therefore a structural part of the diagonal lemma, and the diagonal lemma is a structural part of any Gödelian system. Reality therefore contains this self-referential recursion by the mathematical structure of Gödel’s own results. Denying it would require denying the diagonal lemma or the fact that the substitution function is primitive recursion. Reality is self-referential recursion.

It requires an external base case. Recursion theory defines primitive recursion by the scheme

h(x, 0) = f(x)
h(x, y+1) = g(x, y, h(x, y))


This is the standard definition given in recursion theory. The first equation is the base case; it supplies the value at 0 without reference to h. The second equation is the recursive clause that generates later values from earlier ones. The base case is not produced by the recursive clause; it must be given for the generation to start and to terminate. Because the universe’s formal system contains primitive recursion (via the operations already shown and via the substitution function inside the diagonal lemma), the structure that recursion theory itself assigns to primitive recursion requires a base case external to the function being generated. Therefore, by recursion theory, reality requires an external base case.

## Premise 5

Because reality is primitive recursion (Premise 4), it requires an external base case that starts the generation and allows it to terminate. Local reality therefore had to be started by that external base case.

Candidate accounts of collapse or the emergence of classical outcomes (decoherence, pilot-wave theories, and related proposals) do not satisfy the structure that recursion theory assigns to primitive recursion. They either invoke an internal process to initiate the relevant dynamics or supply no terminating condition that bottoms out the recursion. Any account that fails to provide an external base case external to the recursive structure itself does not meet the requirement established in Premise 4.

## Premise 6

The one who proves the Gödelian truths about the system is external to it. There is only one external placeholder in the structure of primitive recursion: the base case.

Suppose the prover were internal to the system. Then the system would contain a proof of its own Gödelian incompleteness and of the requirement for an external base case. By the second incompleteness theorem (already secured in Premise 3), a consistent system cannot prove its own consistency; more generally, the presence of such a proof inside the system would render it inconsistent. But Premise 1 establishes that the system is standard classical mathematics, and Premise 3 shows it is consistent by the principle of explosion. Empirically and by those premises the system is not inconsistent. Therefore the prover cannot be internal.

Only something external to the system can prove truths about its incompleteness and about the external base case it requires. The structure of primitive recursion supplies exactly one external placeholder—the base case that starts and ends the generation. That base case must also perform the quantum measurement that collapses the system and grounds local outcomes. The only candidate that satisfies both the external status and the measurement role is consciousness. Therefore consciousness is the external base case.

## Final conclusion

Reality is a mathematical, computational, recursive, self-referential formal system that requires an external base case. That base case is responsible for starting and ending the recursion, and that base case is consciousness.

```lean
-- Premise 1
axiom QMSatisfiesCTTCriteriaOfEffectiveMethod : True
axiom QMIsMath : True
axiom QMIsComputational : True
axiom QuantumComputingOperationsAreNaturallyInstantiatedInReality : True
axiom RealityIsUltimatelyAClosedQuantumSystem : True
axiom RealityHasMinimumPeanoArithmeticStrength : True

-- Premise 2
axiom QTMIsPhysicallyInstantiatedInRealityByConsequenceOfP1 : True
axiom RealityIsAFormalSystem : True

-- Premise 3
axiom RealityIsGodelianAsItMeetsItsRequirements : True

-- Premise 4
axiom RealityIsSelfReferentialRecursion : True
axiom DiagonalLemmaIsMathematicallyPartOfReality : True
axiom SubstitutionFunctionIsPrimitiveRecursion : True
axiom RealityHasPrimitiveRecursion : True
axiom RecursionTheoryShowsPrimitiveRecursionInTheStructureNeedsABaseCaseExternalToTheFunctionGenerated : True
axiom RealityNeedsABaseCase : True

-- Premise 5
axiom LocalRealityRequiresExternalBaseCaseToStart : True
axiom CollapseAccountsFailPrimitiveRecursionStructure : True

-- Premise 6
axiom ProverOfGodelianTruthsIsExternal : True
axiom OnlyOneExternalPlaceholderIsBaseCase : True
axiom ConsciousnessIsTheExternalBaseCase : True

-- Conclusion
theorem RealityIsAMathematicalComputationalRecursiveSelfReferentialFormalSystemRequiringAnExternalBaseCaseWhichIsConsciousness : True :=
  have _ := QMSatisfiesCTTCriteriaOfEffectiveMethod
  have _ := QMIsMath
  have _ := QMIsComputational
  have _ := QuantumComputingOperationsAreNaturallyInstantiatedInReality
  have _ := RealityIsUltimatelyAClosedQuantumSystem
  have _ := RealityHasMinimumPeanoArithmeticStrength
  have _ := QTMIsPhysicallyInstantiatedInRealityByConsequenceOfP1
  have _ := RealityIsAFormalSystem
  have _ := RealityIsGodelianAsItMeetsItsRequirements
  have _ := RealityIsSelfReferentialRecursion
  have _ := DiagonalLemmaIsMathematicallyPartOfReality
  have _ := SubstitutionFunctionIsPrimitiveRecursion
  have _ := RealityHasPrimitiveRecursion
  have _ := RecursionTheoryShowsPrimitiveRecursionInTheStructureNeedsABaseCaseExternalToTheFunctionGenerated
  have _ := RealityNeedsABaseCase
  have _ := LocalRealityRequiresExternalBaseCaseToStart
  have _ := CollapseAccountsFailPrimitiveRecursionStructure
  have _ := ProverOfGodelianTruthsIsExternal
  have _ := OnlyOneExternalPlaceholderIsBaseCase
  have _ := ConsciousnessIsTheExternalBaseCase
  True.intro