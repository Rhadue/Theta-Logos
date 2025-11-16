# Contributing to θ-Logos

Thank you for your interest in contributing to θ-Logos!

---

## Ways to Contribute

1. **Domain Applications** - Apply θ-Logos to new domains
2. **Extension Patterns** - Develop reusable extension symbols
3. **Examples** - Add clear, well-documented examples
4. **Documentation** - Improve clarity, fix typos, add explanations
5. **Validation** - Test comprehensibility with fresh users or LLMs
6. **Tools** - Build parsers, validators, or visualization tools

---

## Before Contributing

1. **Read the [Core Specification](theta_logos_core_v1.1.md)**
2. **Review [Examples](EXAMPLES.md)**
3. **Search existing issues** to avoid duplicates
4. **Start small** - simple examples or documentation fixes first

---

## Domain Application Guidelines

When applying θ-Logos to a new domain:

### 1. Start with Core Symbols
Try expressing your domain concepts with the 14 core symbols before adding extensions.

### 2. Document Your Process
Show:
- **Domain context**: What field? What problem?
- **Core attempt**: How far can you get with 14 symbols?
- **Extensions needed**: What patterns repeat?
- **Validation**: Did someone else understand it?

### 3. Example Template

```markdown
## Domain: [Your Field]

### Concept: [What you're describing]

**Using Core Symbols Only**:
```
[∃: A → B → C]
```

**With Minimal Extensions**:
```
Custom symbols:
⊲ = [your symbol meaning]

[∃: A ⊲ B → C]
```

**Validation**: 
- Tested with: [fresh LLM / colleague / etc.]
- Result: [comprehensible / needs refinement]
```

---

## Extension Guidelines

### Good Extensions Are:

✅ **Minimal** - Single symbol for frequently repeated pattern  
✅ **Intuitive** - Meaning guessable from context  
✅ **Documented** - Clear definition + examples + usage notes  
✅ **Reversible** - Can return to core if it doesn't work  
✅ **Validated** - Tested with fresh users

### Avoid:

❌ Creating extensions for single-use cases  
❌ Symbols that only you understand  
❌ Undocumented notation  
❌ Overlapping with existing symbols  
❌ Domain jargon without explanation

### Extension Template

```markdown
### [Symbol]: [Brief Name]

**Symbol**: [Your symbol here]

**Meaning**: [Clear, concise definition]

**Used when**: [Specific contexts where this is needed]

**Domain**: [Which field(s) use this]

**Example**:
```
[∃: A → B ⊕ [symbol]]
```

**Explanation**: [What the example shows]

**Replaces**: [What verbose pattern this compresses]
```

---

## Pull Request Process

### 1. Fork the Repository

### 2. Create a Branch
```bash
git checkout -b feature/your-domain-application
```

### 3. Make Changes
- Add your examples to appropriate files
- Create new files if adding substantial domain work
- Update documentation if needed

### 4. Test Your Changes
- Can a fresh reader understand with just the dictionary?
- Are examples clear and well-formatted?
- Is all new notation documented?

### 5. Commit with Clear Messages
```bash
git commit -m "Add neural network examples with activation notation"
```

### 6. Submit Pull Request
Include:
- **What**: What domain/examples you're adding
- **Why**: What gap this fills
- **Validation**: How you tested comprehensibility

---

## Code of Conduct

### Be:
- **Respectful** - Different domains, different perspectives
- **Constructive** - Suggest improvements, don't just criticize
- **Clear** - Explain your reasoning
- **Patient** - This is experimental work

### Don't:
- Claim ownership of θ-Logos (it's community work)
- Make changes that break existing examples without discussion
- Add proprietary or classified information
- Disrespect other contributors or domains

---

## Questions?

- **General questions**: Open a [Discussion](../../discussions)
- **Bug reports**: Open an [Issue](../../issues)
- **Feature requests**: Open an [Issue](../../issues) with [Feature] tag
- **Documentation fixes**: Submit a Pull Request directly

---

## Recognition

Contributors will be acknowledged in:
- README.md acknowledgments section
- Specific domain documentation (if substantial contribution)
- Release notes (for significant additions)

---

## License

By contributing, you agree that your contributions will be licensed under CC-BY-SA 4.0, the same license as the project.

---

## Philosophy Reminder

> "The language serves the content, not vice versa.  
> Structure emerges from necessity.  
> Trust the evolutionary process."

θ-Logos grows through community use. Your contribution helps it evolve.

Thank you for being part of this journey!

---

**Questions about contributing?** Open a [Discussion](../../discussions) or [Issue](../../issues).
