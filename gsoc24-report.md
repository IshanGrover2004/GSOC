# GSOC 2024 Report
## Project Goal
- Organisation: [CCextractor Development](https://summerofcode.withgoogle.com/programs/2024/organizations/ccextractor-development)
- Project Link: [CCExtractor - Release 1.00](https://summerofcode.withgoogle.com/programs/2024/projects/Jhtnoefj)

[CCExtractor](https://github.com/CCExtractor/ccextractor) is a CLI tool used to produce subtitles for TV recordings which is Open Source and made in C. 

CCExtractor is currently in the process of migrating its existing C code to Rust. This transition is being made primarily for security reasons, while ensuring that the existing C code remains unaffected.  
My project is focused on supporting this migration as part of the effort to finalize the release of CCExtractor 1.00. The key goals of the project include:
1. **Porting C Code to Rust**: A significant portion of the existing C code will be rewritten in Rust to improve security and reliability.
2. **Simplifying CCExtractor Usage**: Created a Docker image to make it easier for users to run CCExtractor without having to worry about environmental setup.
3. **Code Testing**: Added unit tests to all Rust code to ensure its correctness, as well as running regression tests to verify that the overall functionality remains intact.
4. **Resolving Unfinished Work**: The project also involves resolving some previously unfinished pull requests, including work from Elberronnie's previous GSoC work(https://github.com/elbertronnie/gsoc23-report).

## Contributions
- [Pull Request #1611](https://github.com/CCExtractor/ccextractor/pull/1611) -> Create Docker image for CCExtractor
- [Pull Request #1615](https://github.com/CCExtractor/ccextractor/pull/1615) -> Create unit test for rust code
- [Pull Request #1618](https://github.com/CCExtractor/ccextractor/pull/1618) -> Initialize data structures for the rust CEA-708 decoder and correct Dtvcc
- [Pull Request #1621](https://github.com/CCExtractor/ccextractor/pull/1621) -> Create `lib_ccxr` and `libccxr_exports`
- [Pull Request #1622](https://github.com/CCExtractor/ccextractor/pull/1622) -> Add log module in `lib_ccxr`
- [Pull Request #1623](https://github.com/CCExtractor/ccextractor/pull/1623) -> Add time units module in `lib_ccxr`
- [Pull Request #1624](https://github.com/CCExtractor/ccextractor/pull/1624) -> Add constants module in `lib_ccxr`
- [Pull Request #1627](https://github.com/CCExtractor/ccextractor/pull/1627) -> Add bits and levenshtein module in `lib_ccxr`
- [Pull Request #1628](https://github.com/CCExtractor/ccextractor/pull/1628) -> Add encoding module in `lib_ccxr`
- [Pull Request #1629](https://github.com/CCExtractor/ccextractor/pull/1629) -> Add C to Rust code migration guide (just a volunteer work)

## Work left to do
[Pull Request #1618](https://github.com/CCExtractor/ccextractor/pull/1618) has been completed, but some regression tests are still failing. I need to thoroughly investigate these issues to resolve the PR and get it merged.

## Acknowledgements
I want to thank **Carlos Fernandez Sanz** for creating this incredible product and for the opportunity to collaborate with Google Summer of Code.  
I'm also very grateful to my mentors, **Punit Lodha**, **canihavesomecoffee**, and **thealphadollar**, for helping & guiding in contribution. 
A special thanks to Prateek Sunal for collaborating and working with me in this project.
