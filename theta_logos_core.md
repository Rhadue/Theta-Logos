# θ-Logos Core Specification
## Universal Semantic Notation

**Version**: 1.2  
**Date**: 2026-08-01  
**License**: CC-BY-SA 4.0  
**Philosophy**: Minimal core, almost infinite scalability

---

## CORE SYMBOLS (9 primitives)

The core is nine symbols. The six emotional states listed further down are not
additional primitives — they are a **standard vocabulary of labels** on symbol #8,
which carry composition rules of their own. Counting them as primitives would make
the core unbounded, since `θ` accepts any label at all (`θ_catalysis`,
`θ_phase_change`, and so on).

### The colon

Structural operators are written with a trailing colon when they open a clause
inside a block:

```
∃:   ∈:   ⊂:   θ:
```

The colon marks "this operator applies to what follows". It is punctuation, not a
symbol: `∃` and `∃:` are the same operator. Bare forms appear when referring to
the operator itself rather than using it.

`→` and `⊕` are infix and never take a colon.

### Structural Operators (7 symbols)

```
Symbol #1:  ∃   exists, appears
Symbol #2:  ∈   belongs to, is part of
Symbol #3:  ⊂   contains, has substructure
Symbol #4:  →   becomes, transforms to
Symbol #5:  ⊕   together with, combination
Symbol #6:  ≡   equivalent to, results in
Symbol #7:  []  coherent process block
```

### Emergent State Marker (1 symbol)

```
Symbol #8:  θ   threshold, qualitative emergence
```

Can be labeled: `θ_name` for specific emergent properties  
Example: `θ_phase_change`, `θ_catalysis`, `θ_consciousness`

### Negation (added in v1.2)

```
Symbol #9:  ¬   does not exist, has ceased
```

**Usage**: `¬∃[X]` — X does not exist, or no longer does.

```
[∃: Paper ∈: Fire → ¬∃: Paper ⊕ ∃: Ash ⊕ θ_combustion]
```

Reads: "paper exists in a fire context, ceases to exist, ash comes into being,
combustion emerges".

`¬` applies to `∃` and to `∈`. It does not apply to `→`, to `θ`, or to emotional
states: an emergence either occurs or is simply not written.

**Why this exists.** Versions 1.0 and 1.1 had no way to say that something stopped
existing, which made even elementary transformations inexpressible — burning,
dissolution, death. The gap was found empirically rather than by review: in a
multi-model session on the sentence *"a paper burns to ash"*, four models with
different architectures each introduced `¬` unprompted, having no such symbol
available to them. Convergence on the same character by independent systems is the
reason it was adopted in that form rather than another.

### Emotional Atomic States (standard vocabulary, not primitives)

These are six conventional labels on symbol #8, not separate symbols. They are
listed because they recur and because they carry composition rules the general
`θ_name` form does not.

```
θ_joy      pleasure, satisfaction
θ_fear     anxiety, concern
θ_love     attraction, connection
θ_awe      wonder, respect
θ_hope     anticipation, potential
θ_grief    loss, sadness
```

**Composition rules for emotions:**
- Can combine: `θ_courage ≡ [θ_fear ⊕ θ_hope]`
- Can transform: `Challenge → [θ_fear ⊕ θ_hope] → θ_courage`
- **Cannot** have substructures: `θ_fear ⊂: θ_hope` is invalid
- **Cannot** be containers: emotional states are terminal nodes

---

## COMMON PATTERNS (recommended but not required)

These patterns emerge frequently and can be added as extensions:

### Mediation Pattern
```
⟨x⟩  process mediated by factor x
```

**Usage**: `[∃: A → B ⟨factor⟩]` means "A becomes B, mediated by factor"

**Examples**:
- `[∃: Protein → Folded ⟨chaperone⟩]` - folding mediated by chaperone
- `[∃: Signal → Response ⟨receptor⟩]` - response mediated by receptor

### Cycle Notation
```
⟲   cycle completion, return to origin
```

**Usage**: `[∃: A → B → C → A ⟲]` means "cycle completes and returns"

### Indexing Pattern
```
ᵢ   subscript for indexed instances
```

**Usage**: `Aᵢ, A₁, A₂` for multiple instances or iterations

---

## SYNTAX RULES

### Block Structure
```
[∃: X ∈: Y → Z ⊕ θ_result]
```

**Rules**:
1. **Start**: Every block begins with `∃:`
2. **Context**: Followed by `∈:` (belongs to) or `⊂:` (contains)
3. **Flow**: Contains at least one `→` transformation
4. **Emergence**: Can contain one `θ:` or `θ_name` for qualitative change
5. **Nesting**: Blocks can nest for hierarchical structure

### Simple Example
```
[∃: Water ∈: Heat → Steam ⊕ θ_phase_change]
```
Reads: "Water exists in heat context, transforms to steam with phase change emergence"

### Nested Example
```
[∃: System ⊂: [
    [∃: Component_1 → State_1]
    [∃: Component_2 → State_2]
  ] → Output ⊕ θ_emergence]
```

---

## UNIVERSAL PATTERNS

### Pattern 1: Simple Transformation
```
[∃: A ∈: context → B]
```

### Pattern 2: Competition / Alternative Pathways
```
[∃: A → B]
[∃: A → C]
```
A can become either B or C (competing pathways)

### Pattern 3: Cycles
```
[∃: A → B → C → A]
```
Circular process (can add `⟲` if using cycle extension)

### Pattern 4: Hierarchical Structure
```
[∃: System ⊂: [
    [∃: Part_1 → State_1]
    [∃: Part_2 → State_2]
  ]]
```

### Pattern 5: Mediation
```
[∃: A → B ⟨factor⟩]
```
Process mediated by external factor (requires mediation extension)

### Pattern 6: Indexed Instances
```
[∃: Process ⊂: [A₁ → B₁] ⊕ [A₂ → B₂] ⊕ ... ⊕ [Aₙ → Bₙ]]
```

---

## EXTENSION GUIDELINES

θ-Logos is designed to be extended for specific domains. When extending:

### 1. Prefer Core Symbols First
Before creating new symbols, try expressing concepts with the 9 core symbols.

### 2. Domain Extensions Should Be:
- **Minimal**: Add only what's truly needed
- **Intuitive**: Symbol meaning should be guessable
- **Documented**: Every extension needs clear definition
- **Reversible**: Can return to core if extension doesn't work

### 3. Common Extension Types

**Directional operators**: For flow direction (e.g., `⊳` for 5'→3' in molecular biology)  
**Process modifiers**: For specific transformations (e.g., `◊` for energy cost)  
**Domain entities**: Using subscripts (e.g., E₁, E₂ for energy levels)  
**Cycle markers**: Domain-specific cycle notation (e.g., `○` for metabolic cycles)  
**Quantity markers**: For counting (e.g., `×3` for three units)

### 4. Example Extension (Biochemistry)

**Need**: Energy cost in metabolic processes  
**Solution**: Add `◊` symbol for GTP/ATP hydrolysis

**Before**:
```
[∃: Step → Product + energy_cost]
```

**After** (with extension):
```
[∃: Step → Product ⊕ ◊]
```

More compact, clearer meaning.

### 5. Extension Validation
**Test**: Can someone unfamiliar with your domain understand the notation with just your dictionary?

If NO → extension needs better documentation or is too domain-specific.

---

## DESIGN PRINCIPLES

1. **Elegance > Precision > Efficiency**
2. **Universal comprehension** (cross-LLM, cross-domain, cross-human)
3. **Self-documenting structure** (notation + dictionary = complete understanding)
4. **Free evolution** over rigid constraints
5. **Organic patterns** emerge from necessity, not prescription

---

## PROVEN APPLICATIONS

θ-Logos has been validated (via cross-LLM experiments, not peer review) for:
- **Biochemistry**: Metabolic cycles, protein folding, translation
- **Abstract concepts**: Consciousness, purpose, knowledge, emotions
- **Process dynamics**: Multi-agent collaboration, workflows

Expected to scale to:
- Neural networks and perception
- Economic systems and market dynamics
- Physical processes
- Mathematical structures
- Any system with: entities, transformations, emergence

---

## USAGE EXAMPLES

### Simple Process
```
[∃: Input ∈: System → Processing → Output]
```

### With Emergence
```
[∃: Components ⊕ Interaction → Structure ⊕ θ_function]
```

### Emotional State Composition
```
[∃: Challenge ∈: Context → [θ_fear ⊕ θ_hope] → θ_courage]
```

### Complex Nested System
```
[∃: System ⊂: [
    [∃: A → B → C]
    [∃: C → D ⊕ θ_emergence]
  ] → Final_State]
```

---

## VALIDATION METHOD

A θ-Logos description is valid if:

1. **Syntactically correct**: Follows core structure rules
2. **Semantically clear**: Meaning reconstructible from notation + dictionary
3. **Fresh LLM comprehensible**: Naive AI can understand with dictionary alone
4. **Poetically expressible**: Can inspire coherent artistic expression (optional but powerful validation test)

**Example poetic test**:
```
[∃: Code ∈: Cell → Protein ⊕ θ_life]
```
→ Poem: *"From silent code, life sings."*

If notation enables poetry, it captures essence, not just mechanics.

---

## LIMITATIONS

θ-Logos is NOT designed for:
- **Numerical computation**: Use mathematical notation or programming languages
- **Formal proofs**: Use logic systems or proof assistants
- **Real-time execution**: Not a programming language, not executable
- **Precise measurements**: Use scientific notation with units
- **Complete biological accuracy**: High-level conceptual description, not molecular simulation

θ-Logos IS designed for:
- Conceptual clarity across domains
- Structural and processual understanding
- Cross-system communication (AI-AI, human-AI, human-human)
- Pattern recognition and emergence tracking
- Educational and exploratory purposes

---

## CONTRIBUTING

To extend θ-Logos for your domain:

1. **Start with core**: Try expressing concepts with 9 symbols
2. **Identify patterns**: What repeats frequently in your domain?
3. **Create minimal extensions**: Add only necessary symbols
4. **Document clearly**: Each symbol needs definition + examples
5. **Validate**: Test with fresh LLM or naive user
6. **Share**: Contribute extensions back to community (optional)

---

## PHILOSOPHY

> "The language serves the content, not vice versa.  
> Structure emerges from necessity.  
> Trust the evolutionary process."

θ-Logos is not a finished system. It's a seed.  
**Grow it where you need it.**

---

**Maintained by**: Open community  
**Questions**: See examples, documentation, GitHub discussions  
**Citation**: θ-Logos Core Specification v1.1 (2025)
