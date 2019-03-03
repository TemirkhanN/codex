# CODEX

## NO

- Ternary operators (hard testing)
- Fluent interface entities (code polution)
- Variables in quotes (bad visual code-reading)
- {@Inheritdoc} usage (excess parent exploration)
- Public or protected variables (potential prohibited usage)
- Repository can not be used directly for side effect operations.(it should be done via service)
- Setters in models(model methods have to represent actions with affection on state).

## YES

- Clear comments based on ubiquitous language (transparent domain model)
- Everything but testing class is mock (no fooling code coverage; clear tests)*[testing-is-not-that-simple][]
- Repository works with implementation(your interface encapsulates implementation so you won't be able access setters through it).

## Uncertainty

- Avoid embedded entities setters If it is not reasonably necessary(for exmp: DateTimeImmutable). In common it is sufficient to declare embedded entities in constructor and then access them through getters.


[testing-is-not-that-simple]: https://github.com/mockito/mockito/wiki/How-to-write-good-tests#dont-mock-type-you-dont-own
