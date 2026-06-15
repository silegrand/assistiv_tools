# Carer Companion, Concept Document

*A desktop application to reduce the mental load of unpaid caring, so the carer has room to care.*

Assistiv Systems · Concept v1 · For internal development

---

## The mission, stated plainly

A carer's day is not short of love. It is short of *bandwidth*. Every hour spent working out which letter goes with which appointment, re-explaining the same history to a fifth professional, or lying awake wondering whether the thing the physio said contradicts the thing the neurologist said, is an hour and a unit of mental energy taken from the person they are caring for.

This application has one job: **take the administrative and sense-making load off the carer's mind and hold it reliably somewhere else, so the carer can spend their attention on the human in front of them rather than the paperwork behind them.**

Everything below serves that single test. If a feature adds capability but also adds load, it fails the test and does not ship.

---

## Where this came from

The concept began with a real account. A friend whose husband suffered a brain injury described the shape of her days: she had become the unpaid case manager, secretary, advocate, and memory for her husband's entire care, almost entirely without support. Three things came through most sharply.

First, she was **drowning in information**, letters, scan results, emails, discharge summaries, medication changes, appointment cards, with no system that made sense of it, on top of the caring itself.

Second, she could not work out **what to ask**. In the room with a consultant, the right questions only surfaced later, at 2am. The information asymmetry between an exhausted carer and a specialist is brutal, and it is where carers lose the most.

Third, and most telling, **no one was joining the dots**. The neuro team did not see the physiotherapist's notes. The GP did not have the discharge summary. She was the only person holding all the threads, and she was the least equipped, by exhaustion and by training, to see how they connected.

That third point is the heart of this product. A filing cabinet solves the first problem. A good reminder app solves part of the first. But the thing that is genuinely missing, the thing no existing tool does, is **sense-making across fragmented clinical sources on behalf of someone too overloaded to do it themselves.**

---

## The core thesis

Most "carer apps" are organisers: somewhere to store documents and set reminders. They treat the carer's problem as a *storage* problem. It is not. It is a *cognition* problem. The carer's mind is doing four exhausting jobs at once:

1. **Holding**, remembering everything, because they are the only continuous record.
2. **Sorting**, deciding what matters, what is urgent, what can wait.
3. **Connecting**, noticing that two things from two different places might be related.
4. **Advocating**, knowing what to ask, and asking it at the right moment.

Storage tools help only with the first, and only a little. This application is designed to take on all four, with the AI doing the heavy cognitive lifting on jobs 2, 3, and 4, the parts that are currently done badly, late, or not at all, because the carer has no capacity left.

The product is not a medical device and must never behave like one (see *Boundaries*, below). It is a **thinking partner and an organiser of the carer's own information**, pointed squarely at reducing load.

---

## What the application does

The five capabilities below are ordered by how directly they serve the mission. The capture layer comes first because nothing else works if getting information *in* is hard.

### 1. Effortless capture, the load starts at the front door

The single biggest risk to this product is that capturing information becomes another chore. Your friend is already overwhelmed; if she has to carefully file each letter, the app has added load, not removed it. So capture must be close to zero-effort, and forgiving of mess.

- **Drop anything, anywhere.** A scanned letter, a photo of a prescription taken on a phone, a forwarded email, a PDF discharge summary, a voice note dictated in the car park after an appointment. The app accepts it raw and does the sorting itself.
- **The app reads it, not the carer.** On ingest, the AI extracts the useful structure automatically: who it is from (which clinician, which service), what it concerns, any dates, any actions, any medication changes. The carer should never have to fill in a form to file something.
- **Voice-first capture for the moments that matter.** The most valuable information is often what the carer remembers in the moment, not what is written down: "he seemed more confused after the new tablet," "the OT mentioned a referral but I didn't catch to where." A held-button voice note that the AI transcribes and files into the right place captures this without breaking the carer's stride.
- **A forgiving inbox.** Anything the app cannot confidently sort lands in a single, calm inbox, never lost, never demanding. The carer triages only when they have a moment, and the app has already done a first pass.

### 2. The dashboard, one calm surface, the whole picture

This is the home screen, and it is deliberately quiet. An overwhelmed person opening the app should feel *relief*, not a wall of data.

- **The person at the centre.** The dashboard is organised around the cared-for person, not around document types. At a glance: what is coming up, what needs a decision, what is new since last time.
- **A living timeline.** Everything, appointments, letters, medication changes, the carer's own notes, sits on one chronological spine. For the first time, the carer can see the whole journey in one place, and so can any professional they choose to show it to.
- **Today, and only today, by default.** The default view shows what matters now. Depth is available but never forced. The app should never make the carer feel behind.

### 3. The dotted lines, the intelligence that is genuinely missing

This is the differentiating capability and the reason the product exists. The AI continuously looks across everything it holds and surfaces *possible connections that span different sources*, exactly the connections that fall through the gaps between separate medical teams.

- **Cross-source pattern surfacing.** When the neurology letter mentions one thing and the physiotherapy note mentions another that might relate, the app raises it gently: *"The physio noted increased dizziness in March. The new blood-pressure medication started in February. These may be unrelated, but it could be worth asking about together."*
- **Always a question, never a diagnosis.** This is the inviolable rule. The app never says "this is what's wrong" or "these are connected." It says "this might be worth raising" and "here is a question you could ask." It surfaces, the clinician decides. (See *Boundaries*.)
- **Timeline-aware.** Many connections are temporal, a symptom that appeared after a change. The app is well placed to spot "X started shortly after Y" because it holds the dated record no single clinician has.
- **Carer-controllable.** The carer can dismiss a suggested connection, and the app learns not to over-surface. The goal is a small number of genuinely useful prompts, not a stream of anxiety-inducing noise.

### 4. The question builder, closing the asymmetry

The 2am problem: knowing what to ask, and having it ready in the room.

- **Per-appointment question lists.** Before an appointment, the app assembles a short, prioritised list of questions drawn from what has happened since the last visit, what is unresolved, and what connections it has surfaced. The carer walks in prepared instead of remembering on the drive home.
- **Plain-language translation, both directions.** Clinical letters get an optional plain-English summary so the carer understands what was said. And the carer's own observations get help being phrased in the way a clinician will engage with, turning "he's just not right" into "since the last visit he's been more confused in the afternoons and less steady on his feet."
- **Capture the answers too.** A simple way to record what the clinician said in response, so the loop closes and the next question list builds on it.

### 5. Action planning, turning a pile into a path

- **Extracted actions become a gentle plan.** Referrals to chase, forms to return, medications to reorder, calls to make, pulled automatically from letters and notes into one list, with the app doing the "what's next" thinking.
- **Chasing support.** Carers spend enormous energy chasing referrals and waiting on hold. The app can track what has been promised, by whom, and when, and flag what has gone quiet, so the carer knows what to push on without having to hold it all in their head.

---

## Further ideas worth considering

These go beyond the original brief. They are offered as options, not commitments, each is weighed for whether it genuinely reduces load.

**The handover pack.** One tap produces a clean, current summary of the cared-for person's situation, timeline, medications, recent changes, active issues, to hand to a new professional, a respite carer, or A&E. Carers re-tell the same story constantly; this makes them tell it once. *High value, low risk. Strong candidate for early build.*

**The "what changed" digest.** A short, calm weekly read: what is new, what is resolved, what is still open. It gives the carer a sense of being on top of things without having to go looking. *Reduces the background anxiety of "am I missing something."*

**Carer's-own-health nudges.** Heavy-care carers neglect their own health, and carer breakdown is the system's real failure point. Gentle, non-nagging prompts about the carer's own appointments and wellbeing, framed as "you can't pour from an empty cup," not as another task. *Handle with great care, must never feel like surveillance or guilt. Optional, off by default.*

**Shared, permissioned access.** Caring is often shared between family members. Allow a second trusted person to see and contribute, with the cared-for person's consent where possible. *Powerful, but multiplies the consent and data-protection complexity, defer until the single-user model is solid.*

**Benefits and entitlements signposting.** Many carers miss financial and practical support they are entitled to (Carer's Allowance, respite, council assessments). The app could recognise the situation and signpost, not advise, toward what exists. *Signpost only, never assess. Genuinely useful and low-risk if scoped tightly.*

**Connection to the population layer.** Quietly, and only with explicit consent, anonymised and aggregated signals from carers using the app could one day inform the same district-level intelligence Assistiv builds for commissioners, showing where carer load is concentrated in reality, not just in the Census. *A long-horizon idea, mentioned only to note the strategic fit. Behind a strict ethical wall, opt-in, never the product's purpose.*

---

## Design philosophy, calm, not clever

The brief asks for something with the intuitive ease of a well-made Apple application. That instinct is exactly right, and it means something specific here.

**Calm is the primary design goal.** This app is used by people in a state of stress and fatigue. The design's first duty is to lower the heart rate, not to impress. Generous space, one clear thing at a time, soft edges, no clutter, no badges screaming for attention, no red dots demanding action. The emotional target on opening the app is *"I can see everything is held safely, and I know what to do next."*

**The AI is felt, not seen.** The intelligence should show up as quiet, well-timed help, a sorted inbox, a ready question list, a gently surfaced connection, not as a chatbot the carer has to operate. The best version of this product rarely makes the carer *talk to an AI*; it makes the AI do work in the background and present the carer with a calmer, clearer world. A conversational way to ask "what do I need to know about Mum this week?" can exist, but it is a door, not the main room.

**Plain words throughout.** Everything is named by what the carer recognises and controls: "letters," "appointments," "things to ask," "what's coming up", never by how the system is built. No jargon, no clinical coldness, no system-speak.

**Forgiving by default.** Nothing is ever lost. Nothing demands immediate action. Mistakes in filing are easy to fix. The app assumes the carer is doing their best with no time, and is built around that truth.

**Trustworthy by feel.** Because the app holds intimate medical information about a vulnerable person, it must *feel* private and solid at every moment, clear about what it holds, clear that it is the carer's, never doing anything surprising with the data.

---

## Boundaries, the lines this product must not cross

These are not afterthoughts. They are design constraints from the first line of code, and they protect both the people and the product.

**It is not a medical device, and must never act like one.** The moment the app tells someone what is wrong, what to do clinically, or that two things *are* connected, it crosses into regulated medical-device territory (MHRA Software as a Medical Device) and, more importantly, risks real harm, false alarm, false reassurance, or a carer acting on a machine's clinical inference. The discipline is absolute: **the app surfaces questions to raise with a clinician; it never gives a clinical answer.** Every connection is phrased as "worth asking about," every summary carries the clear understanding that it is the carer's record, not medical advice. This framing is what keeps the powerful "dotted lines" feature safe.

**It processes a third party's health data, often without their consent.** The cared-for person may be unable to consent, that is frequently the whole situation. This is a serious data-protection and ethics problem that must be designed for explicitly: the legal basis for holding the data, who owns it, what happens to it, who else can see it, and how the cared-for person's interests are protected even when they cannot speak for them. This needs proper thought and likely proper advice before build, not a checkbox at the end. Assistiv's existing "Iron Curtain" data-siloing thinking is the right starting posture: the carer's and cared-for person's data is theirs, held tightly, never repurposed without explicit, informed opt-in.

**Capture burden is the silent killer.** The most likely way this product fails is not a technical failure or a regulatory one. It is that getting information into it is even slightly too much work for someone already at capacity, so they stop, and the dashboard goes stale, and a stale dashboard is worse than none because it can mislead. The entire design must be ruthless about keeping the cost of capture near zero. This is the bar everything else is measured against.

**Anxiety is an outcome to design against.** A tool that surfaces possible problems can frighten as easily as it helps. The volume, tone, and timing of what the app raises must be tuned to *reduce* the carer's worry, not feed it. Better to surface one genuinely useful prompt a week than ten that read like a list of things that might be going wrong.

---

## How to shape the build

A recommendation on sequence, not a specification.

**Start with the smallest thing that already removes load.** The capture layer plus the timeline plus the handover pack is, on its own, a product worth having, it solves the "drowning in information" problem and the "re-telling the story" problem, which are real and immediate, with low regulatory and ethical exposure. That is the honest first version.

**Add the question builder next.** It is high value, directly addresses the 2am problem, and stays safely on the carer's side of the clinical line.

**Build the dotted-lines intelligence last, and most carefully.** It is the differentiator and the reason the product matters, but it is also where the medical-device line and the anxiety risk live. It deserves to be built on top of a product that is already trusted and already proven to reduce load, with the surfacing tuned conservatively and the "questions not answers" framing locked in.

**Anchor every decision to one person.** Your friend's lived experience is the truest specification this product has. Bring her, or carers like her, into the design from the start. The detail of a real overwhelmed day is exactly what will keep this honest, keep it calm, and keep it from drifting into a clever tool that misses the point.

---

## The test, restated

Before any feature ships, one question: **does this give the carer back mental space, or take more of it?** If it gives space, it serves the mission. If it takes space, however clever it is, it does not belong. A carer who opens this app should feel their shoulders drop, because the load they have been carrying alone is now being held, reliably, somewhere they trust, leaving them free to do the one thing that matters most: care for the person they love.
