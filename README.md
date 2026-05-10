# ClarityAI

ClarityAI is a culturally aware medical communication app built to help patients and families understand clinical conversations, medication guidance, and treatment information in language that feels clear, accurate, and accessible.

## Problem

As children of immigrant parents, we constantly see how the lack of culturally accessible medical information creates profound cognitive overload during stressful hospital stays. When families desperately want to understand medication side effects but face a wall of clinical jargon, that confusion often breeds mistrust. This drives them toward generalized AI models and social media forums that are untrained for medical nuance, ultimately reinforcing harmful preconceptions that can result in lifesaving treatments being rejected.

## Solution

By combining computer science with cognitive science, biology, and linguistics, our solution directly bridges the gap between healthcare and culture. We leverage multi-lingual speech processing alongside a deep understanding of human cognition and clinical biology, creating a truly interdisciplinary tool that dismantles the communication barriers fueling medical inequity.

ClarityAI supports live clinical speech capture, patient-friendly translation, culturally adapted explanations, voice playback, and medication explanations grounded in biomedical context.

## Tech Stack

- React Native / Expo
- Gemini API
- OpenBioLLM-70B via Backboard.ai
- ElevenLabs API
- TypeScript

## Visuals



## Setup Instructions

1. Install dependencies:

```bash
npm install
```

2. Create a `.env` file in the project root with the API keys used by the app:

```bash
EXPO_PUBLIC_GEMINI_API_KEY=your_gemini_api_key
EXPO_PUBLIC_BACKBOARD_API_KEY=your_backboard_api_key
EXPO_PUBLIC_BACKBOARD_PROVIDER=featherless
EXPO_PUBLIC_BACKBOARD_MODEL=aaditya/Llama3-OpenBioLLM-70B
EXPO_PUBLIC_ELEVENLABS_API_KEY=your_elevenlabs_api_key
EXPO_PUBLIC_ELEVENLABS_VOICE_ID=your_optional_voice_id
```

3. Start the Expo development server:

```bash
npx expo start --tunnel -c
```

If Expo returns tunnel or cache errors, start a new terminal, run:

```bash
npx expo
```

Exit that process, then run the tunnel command again:

```bash
npx expo start --tunnel -c
```

## Future Scope

- Expand language coverage and improve support for dialect-specific medical communication.
- Add clinician-facing review controls so providers can verify translated explanations before patients receive them.
- Build medication interaction and allergy checks into the medication explainer.
- Support family-sharing workflows for patients who make decisions with caregivers or relatives.
- Add secure exportable visit summaries for post-discharge review.
- Run user studies with immigrant families and healthcare workers to evaluate trust, comprehension, and cognitive load.

## The Team

- Jason
- Ronin
- Gio
- Kaushik
