[github.com/JheKWall](https://github.com/JheKWall)

---

# General Information

I'm a CSCI graduate from UTM who is working part-time at UTM's ITS Department to continue gathering work experience in the IT field. Besides my programming knowledge in C, C++, C#, Java, Javascript, and Python, I have experience within penetration testing, mobile device management, relational database management, comparative analysis, and network engineering.

I have a passion for game development, which I do in my spare time. Besides that, I've been studying for the CCNA and aiming to take the exam in December to receive CCNA certification to gain more experience in network engineering.

You can reach me at jhekwall@ut.utm.edu (academic inquiries) or wallacejhems@gmail.com (professional inquiries).

You can also find me on LinkedIn at https://www.linkedin.com/in/jhems-wallace/

---

## Analysis Projects

### Student Completion Outcomes at UT Martin and Nearby Institutions (2026)
**Data sourced from [IPEDS](https://nces.ed.gov/ipeds/)**

My goal with this analysis was to measure the completion outcomes of cohorts from 2009-10 to 2016-2017 at UT Martin and nearby institutions alongside cost-of-living data from the same timeframe to determine if there was any credible evidence of a correlation between completion rates and cost-of-living in the area around an institution. This analysis covered eight cohorts (freshmen who entered in the same academic year) across five institutions:

1. Arkansas Northeastern College
2. Dyersburg State Community College
3. Jackson State Community College
4. Murray State University
5. The University of Tennessee at Martin

The analysis yielded the following data:
- Completion rates broadly improved at every institution over the timeframe, with community colleges (two-year institutions) increasing the most.
- UT Martin and Murray State University, the two four-year institutions in the dataset, held a completion rate around ~50% for the entire timeframe.
- Arkansas Northeastern College, Dyersburg State Community College, and Jackson State Community College, the three two-year institutions in the dataset, hold lower completion rates than the four-year institutions. Arkansas Northeastern College proved to be an outlier after its completion rate rose from 28.1% with its 2009-10 cohort to 54.7% with its 2016-17 cohort, exceeding UT Martin's highest completion rate of 52.5%.
- There is no significant correlation between the local cost of living in the immediate area around an institution and the completion rate for a cohort that attended the institution.

Notes and unexpected data:
- Arkansas Northeastern College's increased completion rate is abnormal in comparison to the other two-year institutions, putting it on par with the completion rates of four-year institutions like UT Martin and Murray State University.
- Arkansas Northeastern College's reported living expenses dropped from ~18K+ in 2013-2014 to ~10K+ in 2014-15. This significant drop was less likely to be an actual drop in cost of living around the institution and more likely to be caused by a change in reporting methodology.
- UT Martin did not begin reporting living expenses until 2012-13 (the rest of the dataset starts from 2009-10).

Data sources:
- [IPEDS Complete Data Files](https://nces.ed.gov/ipeds/complete-data-files), National Center for Education Statistics
  - `HD2025` — Institutional Directory (names, sector, county)
  - `OM2017`–`OM2024` — Outcome Measures, eight entering cohorts (2009-10 to 2016-17)
  - `IC2012_AY`, `IC2016_AY`, `IC2019_AY`, `IC2023_AY` — Institutional Characteristics, cost of attendance: living expenses (2009-10 to 2023-24)

Tools used:
- Claude - General assistance and data verification
- Excel - Data storage
- MySQL Server/Workbench - Data storage
- Python (pandas, pytest) - Data analysis, verification
- Power BI - Data visualization

[Read the full report](https://jhekwall.github.io/utm-ipeds-2026/) / [View the report repository](https://github.com/JheKWall/utm-ipeds-2026)

### Comparison of Spacecraft Propulsion Systems (2025)

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

### Comparison of 3D Game Development Engines (2024)

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

## Programming Projects and Assignments

### Unit Testing Implementation for a Banking System



### Programming Databses in WPF Applications



### Threading Experimentation



### Process Management and Scheduling Simulation



---

[github.com/JheKWall](https://github.com/JheKWall)
