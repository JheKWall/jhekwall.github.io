# Analysis Projects

Three self-contained data and research projects. Each has its own repository, its own
write-up, and its own reproducible pipeline.

The common thread across all three is **provenance** — knowing where every number came from,
what it can support, and where it stops. Each project reaches a version of the same
conclusion from a different direction: that a ranking depends on how you cut the data, and
that saying so is more useful than picking a winner.

---

## Student Completion Outcomes Near UT Martin

**IPEDS Outcome Measures · eight entering cohorts · five institutions**

What happens to entering first-time, full-time students at UT Martin and four neighbouring
institutions, how that changed across eight cohorts, and whether local living expenses
appear related to it.

- Completion improved at **every** institution, and most at the community colleges —
  Arkansas Northeastern gained 26.6 points, nearly doubling.
- UT Martin has the **highest transfer-out rate** of the five (23.3%), giving it the highest
  completion-or-transfer rate (75.2%) despite a lower raw completion rate than Murray State.
- **No conclusion about cost is supportable**, demonstrated three ways: the correlation flips
  sign with the choice of cost year (−0.55 vs +0.82), within-institution correlations
  disagree, and pooling produces Simpson's paradox.
- Two data-quality findings surfaced from the charts rather than the aggregates: a 43%
  single-year level break in one cost series, and a transfer-out/unknown split that is
  unreliable year to year.

*Python (pandas) · MySQL · Excel · Power BI · pytest*

[**Read the report →**](https://jhekwall.github.io/utm-ipeds-2026/) · [Repository](https://github.com/JheKWall/utm-ipeds-2026)

---

## Spacecraft Propulsion Systems 2025

**15 systems · 40 individually cited figures · 22 sources**

Which mission role is each category of spacecraft propulsion best suited for? Chemical,
electric, and nuclear compared on specific impulse, thrust, input power, and
thrust-to-weight ratio, separating flight-proven hardware from prototypes and theory.

- **Nothing is best in the abstract, only best for a job.** Chemical is the only category
  that can launch; electric wins sustained efficiency; nuclear occupies an attractive middle
  that has never flown.
- **Ranking on specific impulse alone misleads.** The two highest-scoring systems have never
  been built — one at 2,370× the best hardware ever fired.
- **Thrust-to-weight is computable for only 8 of 15 systems.** The metric that answers "can
  this leave the ground" is the one least often published.
- **A unit error in a peer-reviewed source.** A published table gives antimatter an exhaust
  velocity 333× the speed of light; the same paper's body text gives the correct figure. The
  original transcription was faithful — the error is upstream.

Every figure in the dataset carries its citation, page number, and a verbatim quote of the
sentence it came from.

*Python (pandas) · MySQL · Excel · Power BI · 26 tests*

[**Read the report →**](https://jhekwall.github.io/spacecraft-propulsion-2025/) · [Repository](https://github.com/JheKWall/spacecraft-propulsion-2025)

---

## Game Development Engines 2024

**Senior capstone · CSCI 495 · presented at ACM**

Comparing Godot, Unity, and Unreal Engine from a year of building DATASPIRE, a 3D
first-person action platformer, in Godot.

- Every claim is tagged **built** or **documented**. We used Godot daily for a year; we read
  the other two engines' documentation and never shipped in them. An engine comparison is
  worth reading only if it is clear which parts are experience and which are reading.
- **A five-year feature gap**, verified: Godot's stair-stepping proposal was opened in May
  2021 and is still open, asking for essentially the parameter Unity already ships.
- **A correction to our own conference conclusion.** We told ACM that Godot and Unreal level
  loading were "similarly easy." Our own slide listed three advantages for Unreal. The
  accurate version is that Godot's approach is simpler and Unreal's is more capable.
- **Which engine costs more depends on platform and scale, and the ranking inverts.**
  The engine choice itself was decided by a licensing announcement that was retracted before
  we presented.

*Godot 4.3 · GDScript · Blender · TrenchBroom*

[**Read the report →**](https://jhekwall.github.io/game-dev-engines-2024/) · [Repository](https://github.com/JheKWall/game-dev-engines-2024)

---

[github.com/JheKWall](https://github.com/JheKWall)
