# Status at 27 October 2026

Voyager-X, adaptive force-controlled gripper. Team 11, guide Girish Karikatti.
Portfolio: https://sites.google.com/kletech.ac.in/miniprojectteam11/
Repository HEAD before this update: 159cc3b4efb544473a99ab11427ff2102206ed4f, 15 September 2026.

## Done

- 24 Sep 2026: problem and need statement written; 40 draft functional requirements prepared from a 4 paper literature review.
- 26 Sep 2026: draft set consolidated into 31 functional requirements, 5 non-functional requirements and 5 constraints.
- Literature survey (42 papers in the portfolio rebuild), patent survey (14 patents), market survey.
- 29 Sep 2026: System Composer architecture, 11 components, 8 interfaces, 40 ports, 23 connectors.
- 1 Oct 2026: Simscape CAD plant integration, two compile faults fixed, point masses from STL volumes at 2700 kg per cubic metre, total 0.875 kg. The CAD plant is kinematic with no contact model, so grip force is not proven there.
- 6 Oct 2026: function structure F1 to F7, solution neutral wording, guide sequence fixed.
- 7 Oct 2026: 42 Simulink requirements traced to Review 1 numbers; actuation and sensor calculations.
- 13 Oct 2026: concept selection complete. Mechanism: double slider-crank, r 24 mm, L 45 mm, Fin-Ray fingers. Electronics: bus servo, FSR-408 x2, flex x2, MLX90614, ESP32-S3.
- 23 Oct 2026: portfolio restructured to the HoD hierarchy and filled, handbook items installed (Functional Requirements Table, Foundation Integration Map, Engineering Notebook, Bill of Materials), theme set to Simple Dark, embeds at full width. Final bill of materials 9,795 rupees including GST.
- 26 Oct 2026: 3.5 conceptual design sheets built, version 1 CAD style and version 2 sketch style, plus prompts for AI generation and a Concept C DOCX. Datum, Concept A and Concept B DOCX files were also built. Sheets have not been printed and have not been uploaded to the 3.5 portfolio page.

## In progress, not finished

- Envelope closure: 191 mm against the 150 mm limit. See docs/selection-and-bom.md.
- ESP32-S3 sourcing: only bill of materials line not in any cart at finalisation. See docs/selection-and-bom.md.
- 3.5 title block: full name and USN, and whether sheets are split by student, still to be confirmed.
- Portfolio home gaps: guide email, coordinator name and email, CAD renders, dimensioned drawings, drawn circuit schematic, Gazebo and Simscape screenshots.

## Not started, correctly absent

- Physical prototyping sprints 6.1 to 6.4.
- Testing, section 7, and Step 13 measured verification.
- Debugging and Failure Log: starts at Step 11, minimum 3 cycles by Step 14.
- Dimensioned CAD drawings, section 5.2. The 3.5 sheets are conceptual sketches, not dimensioned drawings.

## Local binary files to upload separately

Text-only GitHub updates cannot carry these. Local copies, checked 27 October 2026:

- `files/gripper_morphological_pugh_selection_v1.xlsx` (old winner-first framing, 13 Oct 2026; the site shows the v2 structure)
- `files/conceptual-designs/` : 3.5 PDFs, DOCX files and combined PDFs, version 1 and version 2
- `workspace/user/files/VoyagerX_Demo.slx`, `VoyagerX_Gripper.slx`
- `workspace/user/files/gripper_mechanism.stp`, `for_mathlab.stp`
- `files/gripper-piper-style/` : STEP and STL files, v3
- `files/gripper-review1-report/build_voyagerx_requirements.m` and related build scripts
- `files/voyager-x-handbook/` and `files/voyager-x-selection/` : HTML embed sources used on the portfolio site

Do not upload the media generation intermediate files in `files/conceptual-designs/` (webp and json sidecars) as evidence. Upload only the finished PDFs, DOCX files and build scripts, after checking each file opens.

## Numbers that must stay consistent everywhere

Objects 20 to 90 mm, up to 250 g. Fragile limit 5 N or less. Rigid hold 8 N or more. Success 90 percent or more over at least 15 objects, 5 trials each. Cycle 6 seconds or less. Supply 12 V DC. Envelope 200 by 150 by 150 mm. Cost cap 20,000 rupees, working target 15,000 rupees, final bill of materials 9,795 rupees including GST.
