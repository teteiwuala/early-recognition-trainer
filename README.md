# Early Recognition Trainer

> **Educational simulation for training purposes only. Not medical advice, not a medical device, and not for clinical decision-making.**

A browser-based simulation that trains nurses to **notice patient deterioration early** — including a voice-commanded VR mode that runs in the Meta Quest browser with no app install.

**[▶ Open the simulation](https://teteiwuala.github.io/early-recognition-trainer/)**

## The problem it targets

The deadliest failure in acute care isn't a lack of knowledge — it's *failure to rescue*. Patients who deteriorate rarely do so without warning; the signs are usually present well beforehand. A climbing respiratory rate, subtle mottling, a patient who is "just a bit off." Nurses learn what these mean. The ones who miss them didn't fail a knowledge test — they didn't look.

Most clinical e-learning tests recall. This trains and **measures noticing**.

## How it teaches

Built on Tanner's Clinical Judgment Model (Notice → Interpret → Respond → Reflect), the framework behind the NCSBN Clinical Judgment Measurement Model used by the Next Gen NCLEX.

- **Looking is a choice.** The vitals monitor is blank until you tap it, and re-masks after four seconds. Attention is logged, never assumed.
- **Nothing announces itself.** Cues appear silently on a schedule that varies slightly every run, so a case can't be beaten by memorising the clock.
- **Reasoning is captured, not inferred.** Scheduled reflection check-ins ask what you notice, what it might mean, and what you'll do — deliberately timed away from cue onsets so a prompt never doubles as an alert.
- **The debrief is the product.** A four-track timeline (Cues / Attention / Actions / Reasoning) on one shared axis makes the gap between *visible* and *seen* impossible to miss, alongside two computed scores — **Time-to-Recognition** and **Cue Latency** (how long the earliest sign was on the monitor before you looked) — and coaching generated from your own session log.
- **It won't flatter you.** The debrief never claims a cue appeared if the run ended first, and escalating before any sign exists is named as a false alarm rather than praised as good instincts.

## Cases

| Case | Setting | What it teaches |
|---|---|---|
| **Quiet Decline** | Surgical ward, post-op day 1 | The core case: sepsis with a rising respiratory rate as the earliest sign |
| **Three Hours Out** *(draft)* | Remote nursing station, no physician on site | The decision clock is **transport** time — escalating early on suggestive findings is correct when the aircraft is hours away |
| **Sugar Crash** *(draft)* | Medical ward, morning round | The key finding is only visible if you think to run a test |
| **Steady Ken** *(draft)* | Surgical ward, pre-discharge | A control case: the patient is fine, and escalating is the *wrong* answer |

Cases marked *draft* are awaiting review by a practising nurse educator. Corrections are welcome and wanted — see below.

## VR mode (Meta Quest)

Open the simulation in the Quest browser and press **Enter VR**. No app store, no developer account, no install — WebXR runs directly in the browser.

In VR you can **speak to the instructor** instead of using controls: *"check his BP"*, *"talk to him"*, *"what have we got in here?"* Interventions require a spoken reason — say *"give him fluids"* and it asks why; say *"give him fluids because his pulse is fading and his palms are sweaty"* and it acts, recording your reasoning to the debrief. Acting for a reason you can state out loud is the difference between judgment and guessing, and it's the whole point.

Voice needs a microphone and an internet connection. Everything else works offline.

## Files

| File | What it is |
|---|---|
| `nurse-sepsis-trainer.html` | The 2D simulation — four cases, briefings, full debrief |
| `nurse-sim-3d.html` | 3D / WebXR version with voice commands |
| `instructor-dashboard.html` | Educator analytics — load exported sessions for class-wide views |

Every file is self-contained: open it directly and it runs. No build step, no server, no accounts, no dependencies to install.

## Privacy

**No student data leaves the machine.** There is no server and no telemetry. Sessions export to a local JSON file the educator keeps, and the dashboard reads those files in the browser. Class codes group sessions for convenience — they are labels, not access control. The optional VR voice feature streams microphone audio to a third-party service and is off unless explicitly enabled.

## For nurse educators

Feedback is the thing this project needs most. If you teach nursing and something here is clinically wrong, imprecise, or pedagogically naive, please open an issue — that's more valuable than any feature request.

## License

MIT — see [`LICENSE`](LICENSE). Provided "as is", without warranty of any kind. The disclaimer at the top of this file applies to every part of this project.
