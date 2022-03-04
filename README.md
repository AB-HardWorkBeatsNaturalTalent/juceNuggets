# juceNuggets

Going through the building blocks for a plugin, publicly.

Goal:
1. A simple application that allows the user to output a MIDI file after fiddling with a slider and pressing export button
2. Sliders shall listen for each other's changes


TODO:
- [X] setup environment to test in a DAW 
- [X] initial setup of GUI app
- [X] add 2 components to view that are notified of changes.
- [X] sliders can react to each other. via lambdas
- [ ] utilize value tree state
- [ ] add export button -> midi file output


Overall plugin architecture notes:

PluginEditor  : what the user sees/interacts with. how the user edits the state.
PluginProcessor : audio DSP here


Test framework:
- [X] use Google Test framework to build test suites 
- [ ] build out an CI/CD pipeline

high level architecture notes:
- the application controller has a model. 
  - the model has an external interface for the controller to use.
- the control components control the model via lambdas
  - the lambdas call the public methods of the model
- we add the control components to the GUI for the user interaction
  - the control components have a look and feel that can be customized.
