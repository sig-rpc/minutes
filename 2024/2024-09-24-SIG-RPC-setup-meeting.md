# 2024-09-24: SIG-RPC Setup Meeting

Initial meeting of people interested in forming the Special Interest Group "Responsible Performance Computing" (SIG-RPC), to formally agree the terms of reference and recruit the founding steering committee prior to it's submission to SocRSE.

This meeting was advertised on SocRSE slack in the `#events` and `#sig-rpc` channels (`#sig-rpc` was earlier advertised in `#general`), after being scheduled via a poll shared in `#sig-rpc`.

## Attendees

- (RC) Robert Chisholm [Chair]
- (NR) Niels Runge
- (RF) Rich Fitzjohn
- (RG) Richard Gilham
- (TM) Tom Mudway
- (JK) James Kilbane
- (WH) Wes Hinsley
- (PH) Peter Heywood

## Agenda/Minutes

- Introductions
  - RC - RSE at Sheffield. Background pure-computer science, performance, optimisation and GPU parallel specialist. Started working on this idea ~18 months earlier, developed ["Profiling & Optimisation (Python)" short course](https://github.com/RSE-Sheffield/pando-python), presented [related talk and notebook](https://rse.shef.ac.uk/pando-python/ppp) at RSECon24. Following the positive feedback to this talk decided to set up this SIG, as there's a much wider scope than can be covered alone. 
  - PH - Similar background to and works in same team as RC, but greater focus on HPC. Has found researchers unaware of concepts such as debug and release builds.
  - JK - Python consultant in finance industry, has been optimising bad Python for several years. Very similar to RC's short-course (he contributed several of the performance patterns), working with Pandas, NumPY etc.
  - NR - Trying to find a career in RSE and attended RC's talk at RSECon24. Hoping to join to see how these problems are dealt with.
  - RF - Head of Imperial's MRC GIDA. Often works on optimisation with a joint interest in getting users with a different profile (e.g. new to Linux) up and running with clusters (e.g. hiding SLURM). Interested in better utilisation of resources and ease of access. Mostly works with R.
  - WH - RSE in RF's team, earlier in career worked with high-performance Java and C, since shifted away from that. Now interested in getting good enough performance, e.g. to not go as deep and stick with the easy wins, getting users off laptops onto HPC/distributed.
  - RG - From Bristol/Isambard AI. Interested to help people get onto platforms bringing with whatever software they have. Helping them to get things up and running, get enough performance to get going without squeezing every last % out. 
  - TM - McMaster university (Canada), formerly in Canada's first centrally funded RSE team. Not had to do much optimisation stuff in the past, but looking to get more involved in performance / build best practices.
- Terms of Reference (TOR) Review
  - Working Draft TOR: https://docs.google.com/document/d/1voERql03hNYWnwPgooiM3PuEHi_TX9OQhqZnUJpMD1Q/edit?usp=sharing *(this link may require changing in future)*
  - Based on template TOR: https://docs.google.com/document/d/1cl_XxFZWwdKvEurPvxUaAeGV8kSxLo5r-Aig_ieJRc0/edit (provided by SIGSIG)
  - Name
    - RC - Initial idea for "Reasonable Performance Computing" was to use the obvious link to "High Performance Computing" grab attention, it also allows for playful conflict. On reflection, considered something along the lines of "Software Performance Best Practices" may be clearer to outsiders.
    - Both names were put to vote, unanimous support to stay with "Reasonable Performance Computing". Various positive comments, such as they would have likely ignored a more serious name and most people are already familiar with HPC so it should be clear.
  - Description
    - RC - The first draft mentioned accessible, however there was a suggestion on SocRSE slack that this could be misconstrued, so preferring to refer to all skill/experience levels.
    - RF - The description misses the "good enough part". 
      - *Action: Final sentence was moved earlier to become second sentence.*
    - RG - Software users not programmers.
      - TM - Suggested "work with software" > "work closely with software"
      - *Action: "closely" was added.*
    - WH - Paragraph concentrates on the code, rather than how to make it so most of their time is research not software stuff, maybe add something to the paragraph to show that it is a low/researcher/developer effort. **"return on investment"**
        - RC - I think "easy performance wins" covers this, but noted.
        - NR - 80:20 rule
        - RC - Donald Knuth's premature optimisation quote
  - Committee Aim
    - RG - "Raising awareness", "Reasonable compute performance"
      - *Action: Reworded to include "to raise awareness of how easy it can be to ensure reasonable performance".*
    - NR -  It should mention general software best practices.
      - RC - Existing software best practices have overlooked performance, only example found was a course that Archer occasionally run. This SIG aims to address that niche.
    - Purpose and Aim of the SIG's outputs
      - WH - An extra point should be added regarding "bridging the gap" between HPC and novice users.
        - *Action: New purpose "work with providers of HPC software and infrastructure to bridge the gap with novice users.*
        - *Note: After the meeting this was later broadened to "work with providers of research computing software and infrastructure, such as HPC, to bridge the gap with novice users." to encompass cloud etc following feedback from PH.
      - JK (*after the meeting*) - It would be easier to sell my involvement to my (industry) clients with a point addressing that materials are not all research specific.
        - *Action: New purpose "where applicable, aim to provide training materials that are broadly applicable, with the aim of allowing people from industries/fields beyond research software to also benefit.*
  - Budget
    - RC - Initial budget proposed zero, all events remote until a community is in place.
    - TM - Everything should be done locally (remotely?).
    - RG - Scope is wide, so budget of zero make sense until we know what community wants / where the success story can come from.
    - NR - New communities tend to grow unexpected, so hard to predict what useful budget would be.
    - WH - agree, but is there anywhere to talk about what will be produced, goals for the new few years.
      - RC - Publicity section covers outputs to some degree. 
  - Insurance
    - No discussion required, to be managed by society.
  - Reporting
    - RC - Keen for docs to be available in markdown via a GitHub organisation, for proper versioning. Wary of shared Google docs with less clear versioning.
      - No objections
  - Committee Roles
    - RC - Recommended 4 members of steering group, but a minimum of 3 is possible, similarly can add extra roles as desired. Majority of the steering group must be SocRSE members, for the SIG to supported by SocRSE. Initial steering group can be decided at this stage (we'll return to this at the end), if any roles unfilled SocRSE will hold election. Future elections held by steering group (e.g. AGM).
    - RF -  Treasurer is redundant with zero budget
      - RC - Just chose the 4 typical roles
      - RF - How about replacing treasurer with editor (e.g. if there is a website)
      - *Action: Treasurer role was replaced with editor.*
  - Equality, Diversity and Inclusivity
    - RF - This is perhaps a chance to broaden the appeal of performance.
    - RG - Diversity comes in many forms, visible and not visible.
  - The Environment and Sustainability
    - RF? - Worth including reduced computing footprint through performance optimisation, that's sustainability.
      - NR - carbon footprint
      - RC - yes, but energy is broader
      - *Action: "The goal of the SIG involves reducing the computing energy footprint, hence benefits sustainability." was added.*
  - Feedback
    - RC - Sheffield is a "Google apps university" so I've defaulted to Google forms here, but happy to broaden.
      - No response
  - Publicity and online presence
    - No comments
- Forming steering committee
  - RC volunteered to **chair**.
  - NR volunteered as **editor**, noted not currently SocRSE but will join if necessary.
  - RF volunteered **deputy-chair** or secretary, whichever remains.
  - PH volunteered as **secretary**, regularly takes minutes at meetings.
  - TM noted, as they're in Canada it would be difficult for them to regularly contribute at this time.
  - Other attendees were offered the chance for roles to be created, but there was no interest.
- Closing
  - RC will set up GitHub org, finalise the terms of reference changes and liaise with James Graham (SIGSIG) and SocRSE to formally submit the proposed SIG for approval by the SocRSE trustees.
  - RC - Following formal approval, will likely organise monthly meetings to move this group forwards. Thanks for your participation
  - *Action: RC to progress things forwards and setup initial infrastructure on behalf of steering group.*
- AOB
  - NR - Thinks it's a really good initiative.
