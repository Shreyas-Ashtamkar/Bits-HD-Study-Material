## Finite Automata

**Finite Automata** are mathematical models that describe discrete state machines. They are used to model the behavior of systems that can exist in a limited number of states and can transition between those states based on input.

**Types of Finite Automata:**

**1) Deterministic Finite Automata (DFA)**

- A DFA is a 5-tuple: (Q, Σ, δ, q0, F)
- Q: Set of states
- Σ: Set of input symbols
- δ: Transition function (Q x Σ -> Q)
- q0: Initial state
- F: Set of final/accepting states


**2) Non-Deterministic Finite Automata (NDFA)**

- An NFA is a 5-tuple: (Q, Σ, δ, q0, F)
- Same as DFA, with the additional property:
    - Multiple transitions exist for a single input symbol in a state.


**Key Concepts:**

**1) State:** Represents the current condition of the system.

**2) Transition:** Represents the change of state based on an input symbol.

**3) Input symbol:** Represents the symbol that triggers a transition.

**4) Final state:** The state in which the system accepts the input string.

**5) Language:** A set of strings accepted by the automaton.


**Deterministic vs. Non-Deterministic:**

- **DFA:** accepts exactly one input string for each possible input.
- **NFA:** can accept multiple input strings for the same input.


**Applications of Finite Automata:**

- **Language recognition:** Identifying natural language patterns.
- **Verification:** Checking if a system meets certain requirements.
- **Compilation:** Translating high-level languages into machine code.
- **Hardware design:** Modeling and debugging digital circuits.


**Example:**

**DFA:** A vending machine that accepts coins and dispenses snacks.
- States: Empty, Coin, Snack, Transaction Complete
- Input symbols: Coin (1, 5, 10), Snack (A, B, C)
- Transition function: Insert coin -> transition to Coin state, Insert snack -> transition to Snack state, and so on.


**NFA:** A spell checker that suggests alternative spellings for misspelled words.
- States: Word, Prefix, Suggested
- Input symbols: Letters, spaces
- Transition function: Match prefix to dictionary -> transition to Suggested state, add letter to prefix -> transition back to Word state.


**Conclusion:**

Finite automata are powerful tools for modeling and analyzing discrete systems. They have numerous applications in various fields and play a fundamental role in the theory of computation.