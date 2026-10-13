# Mac reader kit v1

For the Mac beginner revision of *Git & GitHub for Scientific Computing and Writing*.
Unzip in Downloads, outside your project. This is material to copy, not a repository to clone.
Do not copy the whole kit into your project. It contains no Git automation or history.

## Stages

- Lab 2: start with a new project folder. Copy README.md, then .gitignore, then requirements.txt as the book introduces each file. Finder shows hidden files with Shift-Command-period.
- Lab 3: copy theory/derivation.md and src/analytical.py at their respective steps. The two-line validation guard in step 3.6 remains a small manual edit.
- Lab 4: step02 contains the directly runnable solver; step03 the three-case check; step04 the runner. Copy only the current file into src. Generated outputs are made by running the scripts, not supplied here.
- Lab 5: append readme-run.md to the README. Keep the original problem statement.
- Lab 7: copy warmer-end.md into notes after the warmer experiment, not before.
- Lab 9: insert the two lines in new-cases.txt at the end of CASES, just before its closing square bracket. Keep the three existing cases.
- Lab 11: step03 is text to append to theory/derivation.md. Steps 04–07 each replace exactly one matching file in src. Run checks and commit after each step. Step08 is text to append to README; label the old baseline as v1.0. The prepared runner assumes the Lab 10 baseline: 101 nodes and a 30 C right boundary.
- Lab 12: copy step01 into a new kepler-orbits folder, including .gitignore and .latexmkrc. Record your own requirements-lock.txt after installation; no platform-specific lock is supplied.

## Lab 12 text and figures

`sections/section-00.tex` is Introduction; 01–13 correspond to numbered sections; 14 is Summary. Files contain section bodies only. Replace the matching `% TODO`, preserving the heading and all other sections. The section text is intentionally English in both book editions.

Step05 supplies generate_kepler_data.py for the root. Step07 supplies scripts for figures 1–4 and the matching LaTeX figure blocks. Copy a script into figures, run it, and replace its `% FIGURE N` marker with the corresponding block. Do not copy block files into the project: copy their contents into main.tex.

Step12 supplies figures 5–6 and revision additions. Append third-law-addition.tex to section 10 and variation-addition.tex to section 12, then replace their figure markers. Copy plot-notes.txt and refs.bib to the root. Replace the introduction's `classical problems of mechanics.` line with citation.txt; put bibliography.tex immediately before `\end{document}`. Step14 supplies the single resolved sentence for the planned conflict.

`python build_figures.py` runs only the numbered figure scripts present in the current revision. `python check_data.py` checks the orbit CSV. `latexmk main.tex` uses .latexmkrc to generate build/main.pdf. None performs Git operations. Run them from the project root with its virtual environment active. MacTeX supplies latexmk.

## Checks

Lab 4: three PASS lines and midpoint 60.0 C. Lab 9: five PASS lines.
Lab 11: five PASS lines after steps 4–5, eight after step 6; midpoint 75.0 C after step 7.
Lab 12: 721 orbit samples with radii 0.4–1.6; four figures at v1.0-submitted, six at v1.1-revised.

If a file differs, inspect git diff before replacing it. Stop on unexpected output. The book's recovery guide starts with an external backup. Do not reset a shared branch to match these materials.

The full historical solutions remain at https://github.com/noctis-oss/heat-transfer-1d and https://github.com/noctis-oss/kepler-orbits. They are separate from this starting kit. Their commit IDs are not acceptance criteria for your repository.

## Reuse

Copyright 2026 Yonatan Ali Rodríguez Arias. The supplied code and exercise texts may be used, copied and adapted in your own projects, as permitted for the book's listings. manifest.json records SHA-256 for the packaged files.
