![CAAR Logo](/src/server/static/image/CAARLogo.jpg)

# RotorHazard -> CAAR Adoption
This project evolves over the impressive work from the upstream project. As part of our flight club's adoption (CAAR, Portugal), we are integrating Rotorhazard into the the existing Scoring rules and control system (and not the other way around).

Rotorhazard is the Timing System whereas the score is orchestrated from within MS Excel. Rotorhazard is automated through Excel and results as well as helper data is read from Rotorhazard.

# Rationale and background
The Drone Racing National's Championship in Portugal - aka F9U - is bound to Europe's FAI rules. While addressing FAI's operational rules at events, the Score in Portugal is the result of a community-driven process. Built on the audience input,  the score derives from accumulated points throughout several race events and thus the Championship.

The process is outlined as follows:
 * Qualifiers
    * **Goal**: to generate a *Top 8 leaderboard*
    * Pilots are randomly organized into several groups
    * One round is comprised of several heats.
    * After a complete round, each pilot's points depends on their performance.
    * A minimum of 5 five rounds must be completed. As logistics permits, more rounds represent better odds for all participants.
    * Ambiguous scores are resolved through individual *battle races*.
    * When all ambiguous scores are resolved, the *top 8 pilots* proceed to the Finals
 * Finals
    * **Goal**: Find the Winner through Mini-Finals and Finals heats.
    * Pilots are organized into groups in a pre-defined alignment.
    * An 1/8 Final's heat run takes place
    * **Mini-Finals**: The four 4 pilots with the lower score will dispute the 8-through-5 rank
    * **Finals**: The four 4 pilots with the higher score will dispute the 4-through-1 rank
    * Each of these take two runs.

Entities
 * Federation Aeronautique Internationale [FAI](https://www.fai.org/).
 * Federação Portuguesa de Aeromodelismo [FPAm](http://fpam.pt/home.asp).
 * Clube de Aeromodelismo de Alverca do Ribatejo [CAAR](https://caar-aeromodelismo.com/).


## Changes/additions from the upstream Rotorhazard


* Basic Sports Club branding, visual adjustments only
* WIP


## Contributors
* Paulo Jesus
* Paulo Serrão
* Pedro Fonseca

