# TOFIX

Findings from a code scan on 2026-10-04.

## High

- `README.md:2` - the repo promises "Demos for the Maven build system" but contains no Maven content at all (no `pom.xml`, no Java sources, nothing in git history beyond scaffolding); add the actual demos (with a Maven processor/step in `rsconstruct.toml` so CI builds them) or retire the repo.

## Low

- `README.md:2` - typo "Mavan" (the correct spelling is already in `config/project.lua:3`); also the README is hand-written rather than generated from the fleet `tera.templates/README.md.tera` like the other demos repos.
