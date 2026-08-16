# General Information

I'm a CSCI graduate from UTM who is working part-time at UTM's ITS Department to continue gathering work experience in the IT field. Besides my programming knowledge in C, C++, C#, Java, Javascript, and Python, I have experience within penetration testing, mobile device management, relational database management, comparative analysis, and network engineering.

I have a passion for game development, which I do in my spare time. Besides that, I've been studying for the CCNA and aiming to take the exam in December to receive CCNA certification to gain more experience in network engineering.

You can reach me at jhekwall@ut.utm.edu (academic inquiries) or wallacejhems@gmail.com (professional inquiries).

You can also find me on LinkedIn at https://www.linkedin.com/in/jhems-wallace/

---

## Analysis Projects:

### Student Completion Outcomes at UT Martin and Nearby Institutions (2026)
*Data sourced from [IPEDS](https://nces.ed.gov/ipeds/)*

My goal with this analysis was to measure the completion outcomes of cohorts from 2009-10 to 2016-2017 at UT Martin and nearby institutions alongside institution-reported living expenses from the same timeframe to determine if there was any correlation between completion rates and cost-of-living in the area around an institution.

This analysis covered eight cohorts (freshmen who entered in the same academic year) across five institutions:

1. Arkansas Northeastern College (ANC)
2. Dyersburg State Community College (DSCC)
3. Jackson State Community College (JSCC)
4. Murray State University (MSU)
5. The University of Tennessee at Martin (UTM)

The analysis yielded the following data:
- Completion rates broadly improved at every institution over the timeframe, with community colleges (two-year institutions) increasing the most.
- Between UTM and MSU, the two four-year institutions in the dataset, UTM held a completion rate around ~50% for the entire timeframe while MSU rose to ~60%.
- ANC, DSCC, and JSCC, the three two-year institutions in the dataset, hold lower completion rates than the four-year institutions. ANC proved to be an outlier after its completion rate rose from 28.1% with its 2009-10 cohort to 54.7% with its 2016-17 cohort, exceeding UT Martin's highest completion rate of 52.5%.
- The data cannot support a conclusion that the institution-reported living expenses and the completion rate for a cohort are correlated.

Notes and unexpected data:
- Cohorts are all first-time, full-time freshmen from the same academic year (fall to summer). These cohorts are measured across the next seven academic years.
- ANC's increased completion rate is abnormal in comparison to the other two-year institutions, putting it on par with the completion rates of four-year institutions like UT Martin and Murray State University.
- ANC's reported living expenses dropped from ~18K+ in 2013-2014 to ~10K+ in 2014-15. This significant drop was less likely to be an actual drop in institution-reported living expenses and more likely to be caused by a change in reporting methodology.
- UTM did not begin reporting living expenses until 2012-13 (the rest of the dataset starts from 2009-10).

Data sources:
- [IPEDS Complete Data Files](https://nces.ed.gov/ipeds/complete-data-files), National Center for Education Statistics
  - **HD2025** — Institutional Directory (names, sector, county)
  - **OM2017**–**OM2024** — Outcome Measures, eight entering cohorts (2009-10 to 2016-17)
  - **IC2012_AY**, **IC2016_AY**, **IC2019_AY**, **IC2023_AY** — Institutional Characteristics, cost of attendance: living expenses (2009-10 to 2023-24)

Tools used:
- Claude - General assistance and data verification
- Excel - Reporting output
- MySQL Server/Workbench - Data storage
- Python (pandas, pytest) - Data analysis, verification
- Power BI - Data visualization

[Read the full report](https://jhekwall.github.io/utm-ipeds-2026/) / [View the report repository](https://github.com/JheKWall/utm-ipeds-2026)

### Comparison of Spacecraft Propulsion Systems (2025)
*Data sourced from multiple studies*

My goal with this analysis was to initially determine what the "best" propulsion system was. This quickly changed to determining which mission role each propulsion system was best suited for. I purposefully kept the systems list small (15 total) as I wanted to focus on existing, proven systems. Despite this, I ended up including systems that haven't flown or are purely theoretical as additional information to help create a better analysis.

A brief rundown of the metrics which were measured:
- **Maximum Specific Impulse** (Isp, seconds) - This is the time in seconds it takes for a propulsion system to empty its fuel supply. Generally used as a measure of fuel efficiency alongside other metrics.
- **Maximum Thrust-to-weight Ratio** - Specifically used in the comparison of chemical propulsion systems, this is typically used to help determine whether a rocket system can take off from within Earth's atmosphere.
- **Maximum Thrust** (N) - The maximum amount of force that an engine can output.
- **Maximum Input Power** (kW) - The maximum amount of electrical power needed to run an engine.

The analysis yielded the following data:
- Chemical systems are the only current systems capable of escaping Earth's atmosphere. They do this with a large thrust and a short specific impulse, meaning that they can produce large amounts of force but can only sustain it for a short time.
    - Most Chemical systems are best suited for missions where they are lifting payloads out of an atmosphere or across long distances. However, there are specific Chemical systems which are used for attitude (orientation) correction on space stations.
- Theoretical and tested Nuclear systems are capable of generating even larger amounts of thrust with a longer specific impulse, allowing for travel across longer distances in space.
    - If proven, Nuclear systems would be well-suited for long-distance space travel due to their good thrust and long specific impulse. However, in regards to lifting rockets, there is reasonable concern that Nuclear-powered propulsion systems would not be well-suited for in-atmosphere operation.
- Electric systems are incapable of escaping Earth's atmosphere due to extremely low thrust, but are unmatched in efficient, sustained space travel (albeit at a slower pace) due to a very long specific impulse.
    - Most Electric systems are best suited for satellite propulsion due to their great fuel efficiency. The low speed is less of a concern as satellite components are built to last the duration of their mission.

Notes and unexpected data:
- Each category has their own strengths and weaknesses, with subdivisions within categories further expanding or contracting those metrics. That is to say, propulsion systems are rarely complete upgrades over another propulsion system from another category or even from within the same category.
- It is wrong to rank by a single metric such as specific impulse or maximum thrust as they do not provide enough information to justify any use on their own.
- Thrust-to-weight ratio is only computable for 8 out of 15 systems due to a lack of information (non-published specifications).

Tools used:
- Excel - Reporting output
- MySQL Server/Workbench - Data storage
- Python (pandas, pytest) - Data analysis, verification
- Power BI, Data visualization

[Read the full report](https://jhekwall.github.io/spacecraft-propulsion-2025/) / [View the report repository](https://github.com/JheKWall/spacecraft-propulsion-2025)

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

## Programming Projects and Assignments:

### Unit Testing Implementation for a Banking System



### Programming Databses in WPF Applications



### Threading Experimentation



### Process Management and Scheduling Simulation



---

[github.com/JheKWall](https://github.com/JheKWall)
