# Flugelhorn synthesis

## Usage
  1. Build allolib_playground as per the given instructions
  2. Place flugel.cpp in the same folder as 01_SineEnv_Piano.cpp
  3. Place EnvelopeFlugel.h in the same folder as Envelope.h and OscillatorFlugel.h in the same folder as Oscillator.h
  4. Notelists should be stored in the same folder as notelists for 01_SineEnv_Piano.cpp
  5. To play a song, type "./run.sh tutorials/synthesis/flugel.cpp" while in the root allolib_playground folder

## Demos
  1. Gabriel's Oboe Duet: https://youtu.be/s8SCmGbaD7s
  2. Feels So Good Intro: https://youtu.be/6zZf9w5OSy0
  3. Breathy Sound: https://youtu.be/nCLLUwBSFPU

## High Level Description
  - 15 overtones
  - Sampled real flugelhorn sound
  - Interpolated between overtone series for high notes and for low notes
  - Generated "breathy" effect using filtered white noise
  - Separate envelopes for breathy sound, lower overtones, higher overtones; hope is to make the attacks more realistic-sounding
  - Vibrato with cyclic envelopes for speed and depth

## Future Work
  - It would be nice to add a visual representation for the overtone series of low/high notes.
  - Similarly, a visual representation for each of the envelopes that we can interact with in a tactile manner would be nice.
  - Could we perhaps simulate the physics of a flugelhorn and use this to generate notes instead of using additive/subtractive synthesis?
