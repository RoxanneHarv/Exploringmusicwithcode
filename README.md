# Exploringmusicwithcode
# Song 1
# Start by playing a simple piano tune
# Play the note C (middle C) for 1 beat
playNote(60, beats=1, velocity=80)  # C4
# Pause for half a beat
rest(0.5)

# Play the note E for 1 beat
playNote(64, beats=1, velocity=80)  # E4
# Pause for half a beat
rest(0.5)

# Play the note G for 2 beats
playNote(67, beats=2, velocity=80)  # G4
# Pause for 1 beat
rest(1)

# Repeat with a slight change
# Play the note C again for 1 beat
playNote(60, beats=1, velocity=80)  # C4
# Pause for half a beat
rest(0.5)

# Play the note E again for 1 beat
playNote(64, beats=1, velocity=80)  # E4
# Pause for half a beat
rest(0.5)

# Play the note F for 2 beats (a little different this time)
playNote(65, beats=2, velocity=80)  # F4
# Pause for 1 beat
rest(1)

# More changes to the tune
# Play the note C for 1 beat
playNote(60, beats=1, velocity=80)  # C4
# Pause for half a beat
rest(0.5)

# Play the note D for 1 beat
playNote(62, beats=1, velocity=80)  # D4
# Pause for half a beat
rest(0.5)

# Finish by playing the note G one octave lower for 2 beats
playNote(55, beats=2, velocity=80)  # G3

#acoustic Guitar
# Importing everything from TunePad's chords and constants modules.
# These imports provide the tools I need to create my music project.
from tunepad.chords import *  # Access to functions for playing chords.
from tunepad.constants import *  # Provides useful constants like note durations.

# Setting the key of my song to C major.
# This key is known for its bright and straightforward sound, perfect for calming music.
changeKey("C")

# I'm crafting a simple, soothing chord progression in C major.
# I'll be using the following chords: C major, F major, G major, and A minor.

# Playing the chord progression with a gentle guitar sound.
# The 'rolled' play type gives the chords a soft, real quality that enhances relaxation.
playChord("I", beats=2, velocity=70, playType='rolled', octave=3)  # Starting with C major
rest(1)  # Adding a pause to maintain a relaxed pace
playChord("IV", beats=2, velocity=70, playType='rolled', octave=3)  # Moving to F major
rest(1)
playChord("V", beats=2, velocity=70, playType='rolled', octave=3)  # Then to G major
rest(1)
playChord("vi", beats=2, velocity=70, playType='rolled', octave=3)  # Ending with A minor for a gentle contrast
rest(1)

#dreamy pad Synth
from tunepad.chords import *  # Provides functions for working with musical chords
from tunepad.constants import *  # Contains useful constants like note durations

# I'm setting the key of the song to C major. This is a common key for creating calming music.
changeKey("C")

# Now, I'm going to define a dreamy pad synth line. The idea is to use long, sustained notes
# to create a soothing, atmospheric background for my composition.

# Playing a series of notes to form the pad sound
playNote(C4, WHOLE_NOTE * 2, velocity=50)  # Starting with a C note, played softly
rest(1)  # Adding a short pause between notes
playNote(F4, WHOLE_NOTE * 2, velocity=50)  # Moving to F to add some variation
rest(1)
playNote(G4, WHOLE_NOTE * 2, velocity=50)  # G gives the pad a nice progression
rest(1)
playNote(E4, WHOLE_NOTE * 2, velocity=50)  # Ending the sequence with E for a gentle resolution
rest(1)

#Song 2
#Piano
# Here's the first part of my song using some notes from the C major scale.

playNote(60, beats=1)  # Play C4 for 1 beat - This is the main note to kick things off.

playNote(64, beats=1)  # Play E4 for 1 beat - Moving up, it makes things sound a bit brighter.

playNote(67, beats=2)  # Play G4 for 2 beats - Holding this one longer to wrap up the first little bit.

# Now we go back down to mix it up.
playNote(65, beats=1)  # Play F4 for 1 beat - Taking a step down, switching things up a bit.

playNote(69, beats=1)  # Play A4 for 1 beat - Adds a little bit of tension, like it's leading somewhere.

playNote(72, beats=2)  # Play C5 for 2 beats - Ends on a high note, literally, bringing it all together.

#Electric Bass
# Adding a bass guitar part to go with the piano

# Start with a low C note to match the beginning of the melody
playNote(36, beats=4)  # Play C2 for 4 beats - This just hangs out under the piano.

# Move up to an F note for variety
playNote(41, beats=4)  # Play F2 for 4 beats - Adds some change as the melody moves to F.

# Go back to C to keep things grounded
playNote(36, beats=4)  # Play C2 again for 4 beats - Ends on a steady note as the melody finishes.

#Dreamy Pad synth
from tunepad.chords import *

# Let's create a lush synth pad using the dreamy pad

# Play a C major chord to start (C4, E4, G4)
playNote([60, 64, 67], beats=4)  # Holding this warm chord for 4 beats

# Transition into an F major chord (F4, A4, C5)
playNote([65, 69, 72], beats=4)  # Letting this rich harmony resonate for 4 beats

# Return to the familiar C major chord
playNote([60, 64, 67], beats=4)  # Repeating the soothing C major for another 4 beats

#Song 3
#Piano
# Starting with a simple piano setup

# Play a C major chord (C4, E4, G4) for 4 beats
playNote([60, 64, 67], beats=4)

# Move to an A minor chord (A4, C5, E5) for 4 beats
playNote([69, 72, 76], beats=4)

# Next, an F major chord (F4, A4, C5) for 4 beats
playNote([65, 69, 72], beats=4)

# Finally, a G major chord (G4, B4, D5) for 4 beats
playNote([67, 71, 74], beats=4)

# Simple and straightforward progression to start the song

#Electric Bass
# Adding a bassline to complement the piano chords

# C major bass note (C2)
playNote([36], beats=4)

# A minor bass note (A2)
playNote([33], beats=4)

# F major bass note (F2)
playNote([29], beats=4)

# G major bass note (G2)
playNote([31], beats=4)

# The bassline provides a rhythmic foundation and depth to the music

#Acoustic Guitar
# Adding a melody to enhance the composition

# Simple melody over the chord progression
playNote([72], beats=2)  # C5
playNote([74], beats=2)  # D5
playNote([76], beats=2)  # E5
playNote([74], beats=2)  # D5

playNote([72], beats=2)  # C5
playNote([71], beats=2)  # B4
playNote([69], beats=2)  # A4
playNote([71], beats=2)  # B4

playNote([72], beats=2)  # C5
playNote([74], beats=2)  # D5
playNote([76], beats=2)  # E5
playNote([74], beats=2)  # D5

playNote([72], beats=2)  # C5
playNote([71], beats=2)  # B4
playNote([69], beats=2)  # A4
playNote([67], beats=2)  # G4

# The melody adds movement and interest to the overall piece



