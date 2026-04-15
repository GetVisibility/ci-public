Use these guidelines when generating codeor checking PRs:

## Formatting

- Google Java Format — version from `pom.xml` (`google-java-format.version`)
- Run `mvn spotless:apply` before every commit
- Keep file-level and function-level comments up to date

## Design

— Please follow SOLID, DRY, KISS, YAGNI principles
- Package by Feature: encapsulate functionality within the package scope
- Prefer `Optional` over returning `null` from service methods
- Promote using Lombok where possible
- Constructor injection only — no `@Autowired` field injection
- SLF4J for logging — never `System.out.println`
- Separate request/response DTOs — never expose entities directly
