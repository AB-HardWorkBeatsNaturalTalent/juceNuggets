# juceNuggets

Going through the building blocks for a plugin, publicly.

Goal:
1. A simple application that allows the user to output a MIDI file after fiddling with a slider and pressing export button
2. Sliders shall listen for each other's changes


TODO:
- [ ] setup environment to test in a DAW 
- [X] initial setup of GUI app
- [ ] add 2 components to view that listen to each other: slider 1, slider 2
- [ ] add change broadcast/listeners so sliders can react to each other.
- [ ] utilize value tree state
- [ ] add export button -> midi file output


Overall plugin architecture notes:

PluginEditor  : what the user sees/interacts with
PluginProcessor : audio DSP here
