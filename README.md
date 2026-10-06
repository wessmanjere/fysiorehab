# fysiorehab – Seuraa hahmoa

Mobile-first demo of a follow-the-avatar exercise for knee rehabilitation after surgery, part of an asynchronous remote rehabilitation concept. The patient exercises at home; the physiotherapist reviews the results later.

**Live demo:** https://wessmanjere.github.io/fysiorehab/

- The patient's digital twin (Three.js) shows the target movement as keyframes and only advances when the patient matches each angle within tolerance (±8°, held 0.4 s).
- On-device pose estimation with MediaPipe Pose Landmarker. Video never leaves the device, only joint angles.
- Exercises: Kantapääliuku, Istuen polven ojennus, Suoran jalan nosto, Minikyykky. Prescription is a JSON config at the top of the script.
- Real-time feedback (colour, short Finnish cues, pre-recorded neural voice, haptics), summary with angle chart, pain rating and a mocked send to the physio.
- **Demotila:** simulated patient for presentations without a camera.

Single self-contained `index.html`. The camera needs HTTPS (GitHub Pages works).

Voice cues were generated with the fi-FI Noora neural voice for demo purposes; regenerate them with a licensed Azure Speech account before production use.
