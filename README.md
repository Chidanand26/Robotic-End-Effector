# Adaptive Force-Controlled Robotic End-Effector

Department of Automation and Robotics, KLE Technological University, Hubballi.
Semester V Mini Project, Academic Year 2026-27.
Theme 2: Robotic End-Effector and Manipulation Systems.
Guide: Girish Karikatti.
Team 11: Chidanand (01fe24bar027@kletech.ac.in), Srushti, Lakshmi, Shiddhanth.
Artefact: Force-Controlled Gripping System, called Voyager-X, an adaptive force-controlled gripper.

Portfolio (evidence site): https://sites.google.com/kletech.ac.in/miniprojectteam11/

## Current design, as selected 13 October 2026

The guide selection flow is calculations, then morphological chart, then Pugh chart, then selection. Component names are used in review documents from this point onward.

Mechanism: double slider-crank linkage, crank radius 24 mm, link length 45 mm, 90 mm jaw travel, 20 to 160 degree sweep, with compliant Fin-Ray style fingers. This is Concept A in the 3.5 conceptual designs. The fallback is Concept B, rack and pinion.

Electronics: STS3215 class serial bus servo, two FSR-408 force sensors (0.2 to 20 N), two 2.2 inch flex sensors, MLX90614 infrared temperature sensor, ESP32-S3 controller, dual buck regulators from a 12 V DC supply, MGN9H linear rail guide.

## Superseded note, please read first

The README and wiki files committed on 15 September 2026 describe an earlier concept using a load cell, HX711 and a stepper tendon drive. That concept is superseded by the selection above and must not be used as the current design. The wiki folder in this repository is the 15 September draft outline. The current, checked record is in `docs/` in this update and on the portfolio site. Do not mix the two sets of hardware descriptions in review documents.

## Status at 27 October 2026

Done: problem and need definition, literature survey, patent survey, market survey, requirements (31 functional requirements, 5 non-functional requirements, 5 constraints), design calculations, morphological chart, Pugh charts and concept selection, final bill of materials, System Composer architecture, Simulink requirements traceability, Simscape CAD plant, 3.5 conceptual design sheets (version 1 CAD style and version 2 sketch style), Engineering Notebook to 26 October 2026.

Not done: physical prototyping sprints, subsystem testing (Step 11 onward), Step 13 measured verification, Debugging and Failure Log (starts at Step 11, minimum 3 cycles by Step 14), dimensioned CAD drawings for section 5.2, drawn circuit schematic when wiring is frozen.

Open, honest items: envelope height is 191 mm against the 150 mm limit, so the Concept A selection is conditional until the fingers are shortened, the servo is recessed, or the guide relaxes the limit. The ESP32-S3 line in the bill of materials is a 650 rupees workbook estimate and was not in any vendor cart at finalisation. The full name and USN for the 3.5 title block are still to be confirmed by Chidanand. Guide email and coordinator name and email for the portfolio home page are still missing.

See `STATUS.md` for the full done and not done list.

## What this repository holds after this update

- `README.md`: this file.
- `STATUS.md`: current state at 27 October 2026.
- `docs/requirements.md`: FR-01 to FR-31, NFR-01 to NFR-05, C-01 to C-05.
- `docs/selection-and-bom.md`: morphological and Pugh summary, final bill of materials.
- `docs/calculations-and-models.md`: governing calculations and simulation models.
- `docs/conceptual-designs-3-5.md`: 3.5 sheets, versions, print note and known caveats.
- `wiki/`: 15 September 2026 draft outline, superseded in the respects noted above.
- Root files from 15 September 2026: handbook PDF and Review1_Documentation.xlsx, as first committed.

## Files that cannot be pushed through the text-only connector

Binary files are not in this text update: the selection workbook (.xlsx), the 3.5 PDFs and DOCX files, Simulink models (.slx), STEP and STL files, and the handbook PDF already in the repository. Upload those through a local git clone or the GitHub web upload, from the local copies listed in `STATUS.md`. Do not claim the repository is complete until those files are present, and do not upload a file whose contents have not been checked.

## How to keep this repository current

Update `STATUS.md` and the relevant `docs/` file after every working session, in the same way the Engineering Notebook is updated. Record measured results only after Step 13 testing, never before. Keep the portfolio site and this repository consistent on numbers: object size, force limits, envelope, cycle time and bill of materials total.
