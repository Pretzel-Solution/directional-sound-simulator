# directional-sound-simulator
Use HRIRs to simulate sound coming from different directions.

In this repository a noise and speech signal is provided.
You can also add your own mono sound signal sampled with 48kHz.

The function get_stereo() creates a stereo wav file simulating a sound signal coming from a defined direction.
The function get_roundabout() simulates sound stepping around the head. 
Important: The effect comes ONLY with headphones!
You can hear an example of voice virtually going 360 degree around your head.

Theory:
A head related impulse response (HRIR) is measured by a microphone placed in the ear canal. Sound impulses are created at different directions. For each direction there is a different impulse response in the ear canal measured by the microphone. So for every direction in the database there is an imuplse response for the left and right ear. If a speech signal is convolved with the left and right HRIR from a certain direction, the result is what would reach the left and right ear canal, if the voice comes from this certain direction. This simulates sound from a certain direction.

References:
HRIR Database in SOFA format
http://sofacoustics.org/data/database/thk/HRIR_FULL2DEG.sofa

[15] J. Arend, A. Neidhardt, and C. Pörschmann, “Measurement and perceptual evaluation of a spherical near-field hrtf set”, Nov. 2016.
