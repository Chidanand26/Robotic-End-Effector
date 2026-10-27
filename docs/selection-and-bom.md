# Selection and bill of materials

Selection completed 13 October 2026. Guide sequence: calculations, morphological chart, Pugh chart, selection. Version 2 selection pages were published on the portfolio site on 23 October 2026, with datum counts and mandatory screens. The local workbook `gripper_morphological_pugh_selection_v1.xlsx` still carries the old winner-first framing and the 8,044 rupees estimate, and has not been synced to version 2.

## Mechanism

Datum for Pugh 1: lead screw concept. Concept A, double slider-crank linkage with Fin-Ray fingers, won Pugh 1 at plus 8, against plus 3 for rack and pinion and plus 1 for belt drive, on force headroom, travel and cycle time.

Conditional selection: Concept A fails the mandatory envelope screen, 191 mm against the 150 mm limit. The selection stays conditional until the fingers are shortened, the servo is recessed, or the guide relaxes the limit. Concept B, rack and pinion with MG996R, is the fallback.

Concept set in 3.5: Datum, lead screw with MG996R. Concept A, double slider-crank with STS3215 class bus servo. Concept B, rack and pinion with MG996R. Concept C, belt drive with NEMA 14 stepper and TMC2209. Drive and transmission vary; Fin-Ray fingers, FSR-408, flex sensors, MLX90614, ESP32-S3 and dual bucks are held common so the mechanisms compare like for like.

## Electronics

Concept S2 and S3 were screened out. S2 has only 3 ADC channels for 4 needed and no deformation sensing. S3 has no deformation sensing. The selected electronics won Pugh 2 at plus 19, against plus 2 for Pico W and plus 0 for classic ESP32.

Selected: STS3215 class serial bus servo, FSR-408 x2, flex 2.2 inch x2, MLX90614, ESP32-S3.

## Final bill of materials, 23 October 2026, 9,795 rupees including GST

Prices are vendor cart prices including GST, not confirmed orders, except the ESP32-S3 line noted below. Total is 5,205 rupees under the 15,000 rupees target and inside the 20,000 rupees cap.

- Robocraze, 4,646 rupees: Waveshare 20 kg cm bus servo 2,359, MLX90614 925, DFRobot multi-output buck 619, flex 2.2 inch 253 x2, TPS5430D 3 A buck 237.
- Pricio, 1,514 rupees: SOUSHINE FSR-408 757 x2, free delivery.
- Novo3D, 1,585 rupees: MGN9H blocks 520 x2, MGN9H 400 mm rail 545. Rail decision settled by purchase: MGN9H.
- 3D printing cap, 1,400 rupees, team figure.
- ESP32-S3, 650 rupees, workbook estimate only, not in any cart.

Flags: the TPS5430D servo buck is rated 3 A against the 5 A rail assumed in calculations. Stall draw is about 2 A, about 1.5 times margin, and the force loop caps drive. The Novo3D cart is under the 2,000 rupees free shipping line, so shipping may add at checkout.

ESP32-S3 sourcing, still open at 27 October 2026: verified options were Hubtronics Waveshare ESP32-S3 Mini at 635 rupees with USB-C adapter board, build total 9,780 rupees, and Zbotic Waveshare ESP32-S3 board at 972 rupees, build total 10,117 rupees. No choice has been confirmed. Do not mark the bill of materials as ordered until the ESP32-S3 order is confirmed.
