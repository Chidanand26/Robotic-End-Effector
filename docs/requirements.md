# Requirements

Source: Review1_Documentation.xlsx, consolidated 26 September 2026. Handbook table frozen at Review 3. Verified column is filled only after Step 13 testing, from measured results.

Quantified design inputs: object size 20 to 90 mm, weight up to 250 g, fragile peak force 5 N or less, rigid holding force 8 N or more sustained, at least 15 object types with 5 trials each, success 90 percent or more, cycle 6 seconds or less per object, temperature monitoring up to 100 degrees C.

## Functional requirements

- FR-01: limit peak gripping force on fragile objects to 5 N or less.
- FR-02: hold rigid objects of 200 g or more for 15 s without slip.
- FR-03: grasp objects of characteristic size 20 to 90 mm.
- FR-04: handle objects up to 250 g without dropping.
- FR-05: grasp success rate 90 percent or more across 15 or more object types.
- FR-06: complete grasp, transport and release within 6 s per object.
- FR-07: minimum finger to object contact area 100 mm2 per finger during holding.
- FR-08: detect contact force using the force sensor before exceeding the 5 N fragile limit.
- FR-09: monitor temperature of object and contact region up to 100 degrees C.
- FR-10: maintain stable grasp of a fragile object at 5 N or less through the complete pick and place operation.
- FR-11: adjust finger position for diameter variation of at least 50 mm.
- FR-12: maintain commanded gripping force within plus or minus 0.5 N during holding.
- FR-13: detect temperature changes of 2 degrees C or greater during handling.
- FR-14: record force and temperature data at intervals of 1 s or less through each grasp cycle.
- FR-15: return both fingers to the fully open reference position with error 2 mm or less after release.
- FR-16: detect loss of contact within 0.5 s of a slip event.
- FR-17: reduce applied force to 1 N or less during release.
- FR-18: complete 10 consecutive grasp, hold and release cycles without manual repositioning.
- FR-19: limit relative displacement between object and finger surfaces to 3 mm or less during holding.
- FR-20: open both fingers to minimum clearance 100 mm before approach.
- FR-21: maintain minimum 5 mm clearance between finger mechanism and object body during approach.
- FR-22: finger position repeatability plus or minus 2 mm over 10 consecutive cycles.
- FR-23: detect unsuccessful grasp when force stays below 1 N for 1 s after the grip command.
- FR-24: initiate release within 0.5 s after the release command.
- FR-25: maintain continuous temperature sensor contact for at least 90 percent of handling duration.
- FR-26: provide minimum 2 point contact before lifting.
- FR-27: recover from failed grasp by reopening fingers by at least 80 mm before retry.
- FR-28: complete finger opening to release position within 1.5 s after release command.
- FR-29: maintain measured temperature within plus or minus 3 degrees C of initial contact temperature during a 15 s holding test.
- FR-30: identify stable grasp when force stays within plus or minus 10 percent for at least 1 s.
- FR-31: prevent further closing when temperature sensor measures 100 degrees C or above.

## Non-functional requirements

- NFR-01: conceal internal wiring, target 90 percent or more concealed.
- NFR-02: no loose wires, cables or connectors exposed, target 0.
- NFR-03: smooth external surfaces, no exposed sharp edges, target 0.
- NFR-04: uniform external finish, target 90 percent or more of visible surfaces consistent.
- NFR-05: access sensors and connections without complete disassembly, within 5 minutes.

## Constraints

- C-01: low voltage supply not exceeding 12 V DC.
- C-02: prevent further closing at 100 degrees C or above.
- C-03: fit within 200 by 150 by 150 mm envelope. Open: current Concept A height is 191 mm, see docs/selection-and-bom.md.
- C-04: materials withstand continuous operation up to 100 degrees C.
- C-05: total component cost not exceeding 20,000 rupees.

Note on the site: the Specifications page carries 30 to 70 mm as the object size range in one place. The Review 1 sheet and this requirement set use 20 to 90 mm. Do not change the Review 1 sheet to 30 to 70 mm without the team's word. The 30 to 70 mm propagation question remains open.
