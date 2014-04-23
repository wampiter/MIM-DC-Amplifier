Eagle files for DC amplifier

Currently known issues:
SERIOUS ISSUES:
P-CR and P-CN Must be electrolytic capacitors! 
Slide switches (A-SWITCH and B-SWITCH) are not connected correctly!
If you're not using an op-amp DON'T FLOAT IT! It will oscillate and suck current and do nasty things! Set it up as a follower to ground (or something).
Grayhill switches are actually a slightly different size!

Less serious issues:
The LPF op-amp (NTE928M2A) is floated partially then the switch is off. This could be avoided and a spdt switch could be used instead by simply switching the input of the next stage between the two possible inputs.
Tiny surface mount trimmer resistors are silly and slide switches are just silly.
Electrolytics at input should also have parallel ceramic caps
Use of 723s is silly. Use of a specialized power regulator would save space, complexity, money, and be more precise.
Output BNCs should have solder points for support posts (or perhaps use a different case style completely)
Silk screening should be legible!
Vias should never be within a mm of a solder pad for hand assembly (there are lots) Those almost under components are particularly problematic.
Placement of some components like PN-R5 is silly and out of the way. This board could have many fewer vias and lines, resulting in better performance at high frequency, cheaper manufacturing, and easier building/debugging.
Pay attention to input impedance! If the input is supposed to actually have 50 ohm impedance it should probably have an RC to send high-frequency to ground after input 50 ohm resistor. This needs to be close to the input and/or use stripline.
100u capacitors need bigger case size.
Usability: switches should have some kind of labeling or labellability.
