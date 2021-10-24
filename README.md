# EAGLE-teardrops-w-smd

I realized that the Eagle teardrop.ulp script creates teardrops only on vias and pads but not on SMD footprints.
I added this functionality with the existing logic by utilizing a little trick. First I read the dx and dy values from the SMD pad in question.
Then I take the shorter value and imagine a circle in the center of the pad with the shorter value.
This is our diameter, the drill is just arbitrarily fixed at diameter divided by two. This worked fairly well for my boards so far!
Any feedback is welcome.
