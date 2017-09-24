# CODEX

## NO

- Ternary operators (hard testing)
- Fluent interface entities (code polution)
- Variables in quotes (bad visual code-reading)
- {@Inheritdoc} usage (excess parent exploration)
- Public or protected variables (potential prohibited usage)
- Repository can not be used directly for side effect operations.(it should be done via service)

## YES

- Clear comments based on ubiquitous language (transparent domain model)
- Everything but testing class is mock (no fooling code coverage; clear tests)
- Repository works with implementation(your interface encapsulates implementation so you won't be able access setters through it).

## Uncertainty

- Avoid embedded entities setters If it is not reasonably necessary(for exmp: DateTimeImmutable). In common it is sufficient to declare embedded entities in constructor and then access them through getters.
