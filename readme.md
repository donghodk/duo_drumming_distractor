# SMS Distractor - Max/MSP MIDI data controller

The SMS distractor is a standalone Max/MSP patch, developed to control, manage, and collect MIDI data during the duo-drumming experiments conducted in 2021 at the RITMO Centre for Interdisciplinary Studies in Rhythm, Time and Motion, University of Oslo, Norway.

This patch provides real-time interaction with MIDI input/output and structured data capture for experimental analysis.


# MIDI data format

The collected MIDI data is structured in the following format:

index, timestamp pitch(label) velocity take# distractor_pitchtype distractor_timetype

- index: Event number in sequence.
- timestamp: Time of the event (in milliseconds).
- pitch (label): Used to identify specific drummers or experimental subjects.
- velocity: Intensity of the MIDI note.
- take#: Current experimental take or session ID. This value can be manually entered in the patch.
- distractor_pitch_type & distractor_time_type: Values are arbitrarily numbered for reference and represent one of the experimental variables. This field can be manually set in the patch.
