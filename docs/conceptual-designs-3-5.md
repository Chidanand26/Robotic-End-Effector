# Conceptual designs, section 3.5

Built 26 October 2026. One design per A4 page, printed on 100 gsm paper, parts labelled, guide signature and date line for Girish Karikatti. Sheets are conceptual sketches, not to scale and not dimensioned drawings. Dimensioned CAD belongs in section 5.2.

## Version 1, CAD style

Four one-page A4 PDFs plus a combined 4 page PDF. AI 3D renders were generated with no text in the image, then labels and callouts were drawn in the PDF so labels stay sharp. Labelled parts are morphological chart options. Drive and transmission vary; Fin-Ray fingers, FSR-408, flex sensors, MLX90614, ESP32-S3 and dual bucks are held common.

- Datum: lead screw with MG996R.
- Concept A: double slider-crank with STS3215 class bus servo.
- Concept B: rack and pinion with MG996R, fallback.
- Concept C: belt drive with NEMA 14 stepper and TMC2209.

## Version 2, sketch style

Rebuilt in the style of the reference sheets shared by the team: Datum as a pencil sketch, Concept A as an exploded view, Concept B as a coloured hand sketch, Concept C as a coloured hand sketch. Combined 4 page sketch PDF and `prompts-for-AI-generation.md`, one prompt per concept, are in the same folder. Version 2 fixes slips in the references instead of copying them, for example the duplicated pinion label and vague controller in the Concept B reference.

Known caveats: Concept C in version 2 renders the fingers doubled in perspective and reads as four fingers, not two. The version 1 CAD Concept C sheet remains the clean two finger alternative. Datum version 2 has no separately drawn MLX90614 module; its legend flags that explicitly.

Concept C was also delivered as an editable Word file, image set at 120 mm wide, verified as one A4 page. Datum, Concept A and Concept B DOCX files were built the same way.

## Status

Sheets have not been printed and have not been uploaded to the Google Site 3.5 page. Do not print until two questions are confirmed: the exact full name and USN for the title block, sheets currently say Chidanand only, and whether sheets are split by student, since the reference images name Lakshmi on Concept B and Srushti on Datum.
