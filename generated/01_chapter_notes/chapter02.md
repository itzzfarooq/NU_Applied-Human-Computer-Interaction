# Chapter 2: The Computer - HCI Notes

## Overview
Chapter 2 covers the computer side of HCI: output devices (displays), input devices, text and graphics displays, colour, and other I/O modalities (audio, haptic, pen, keyboard). Understanding computer capabilities and limitations is essential for effective interface design.

---

## 1. OUTPUT DEVICES

### Display Technology
- **CRT (Cathode Ray Tube)** – traditional monitor, electron beam excites phosphors
- **Flat panel displays** – LCD, plasma, OLED
- **Resolution** – number of pixels (horizontal × vertical)
- **Colour depth** – number of bits per pixel (1-bit = B&W, 8-bit = 256 colours, 24-bit = true colour)

### Display Characteristics
- **Luminance** – brightness of display
- **Contrast** – difference between brightest white and darkest black
- **Refresh rate** – how often display is redrawn (flicker if too low)
- **Gamma** – nonlinear relationship between pixel value and luminance

---

## 2. TEXT AND GRAPHICS DISPLAYS

### Text Displays
- Characters generated from fixed matrix (e.g. 5×7 dots)
- Limited character set
- Fast to render
- Limited typography

### Graphics Displays
- Each pixel individually addressable
- Can display arbitrary shapes, fonts, images
- Requires more memory and processing
- Anti-aliasing smooths jagged edges

### Character Entry
- **QWERTY keyboard** – standard layout, designed to prevent jamming
- **Dvorak layout** – optimized for efficiency, less common
- **Chord keyboards** – multiple keys pressed simultaneously
- **Soft keyboards** – on-screen, for touch/pen input

---

## 3. INPUT DEVICES

### Keyboards
- Most common input device
- Various layouts (QWERTY, Dvorak, etc.)
- Function keys, modifier keys, cursor keys
- **Advantages**: Familiar, fast for text entry
- **Disadvantages**: Not natural, requires learning

### Pointing Devices

#### Mouse
- Most common pointing device
- Mechanical (ball), optical, laser
- Measures relative movement
- **Advantages**: Direct manipulation, familiar
- **Disadvantages**: Requires flat surface, one-handed

#### Trackball
- Stationary version of mouse
- Ball on top, moved with fingers/palm
- **Advantages**: Compact, good for limited space
- **Disadvantages**: Less precise than mouse

#### Touchpad
- Surface senses finger position
- Common on laptops
- **Advantages**: No moving parts, portable
- **Disadvantages**: Small area, less precise

#### Joystick
- Lever controls position/direction
- Used in gaming, CAD, simulation
- **Advantages**: 2D/3D control, intuitive
- **Disadvantages**: Fatigue, less precise for text

#### Pen/Stylus
- Direct input on screen surface
- Used in tablets, PDAs,签名 pads
- **Advantages**: Natural writing/drawing
- **Disadvantages**: Occlusion, fatigue

---

## 4. COLOUR

### Colour Models

#### RGB (Red, Green, Blue)
- Additive colour model
- Used in displays
- Each channel 0-255 (8 bits)
- 24-bit = 16.7 million colours

#### HSB/HSV (Hue, Saturation, Brightness/Value)
- More intuitive for users
- Hue: colour type (0-360°)
- Saturation: purity/intensity
- Brightness/Value: lightness

#### CMYK (Cyan, Magenta, Yellow, Key/Black)
- Subtractive colour model
- Used in printing
- Pigments absorb light

### Colour in Interface Design
- Use colour meaningfully and consistently
- **Red** – warning, error, stop
- **Green** – okay, go, success
- **Blue** – information, links
- Consider colour blindness (8% males, 1% females)
- Don't rely on colour alone – use other cues

### Display Colour Issues
- **Gamma correction** – compensates for nonlinear display response
- **Colour calibration** – ensures consistent colour across devices
- **Metamerism** – different spectral compositions can appear same colour

---

## 5. AUDIO OUTPUT

### Types
- **Speech synthesis** – text-to-speech
- **Earcons** – musical sounds representing actions/objects
- **Auditory icons** – real-world sounds (e.g. trash can crumple)

### Applications
- Accessibility (visually impaired users)
- Alerts and notifications
- Navigation feedback
- Entertainment

### Design Considerations
- Speech is slow but attention-getting
- Non-speech audio can be faster
- Cultural differences in interpretation
- Volume control essential

---

## 6. HAPTIC OUTPUT

### Types
- **Vibration** – tactile feedback
- **Force feedback** – resistance to movement
- **Texture simulation** – surface roughness

### Applications
- Mobile phone alerts
- Game controllers
- Surgical simulation
- Accessibility

---

## 7. OTHER INPUT MODALITIES

### Speech Recognition
- Converts spoken words to text/commands
- Types:
  - **Speaker-dependent** – trained to specific voice
  - **Speaker-independent** – works with any voice
  - **Discrete** – one word at a time
  - **Continuous** – natural speech
- Challenges: noise, accent, vocabulary, accuracy

### Gesture Recognition
- Detects and interprets body movements
- Technologies: camera-based, glove-based, accelerometers
- Applications: sign language, gaming, VR

### Eye Tracking
- Tracks eye position and movement
- Measures fixations, saccades, scan paths
- Applications: accessibility, research, advertising

### Brain-Computer Interface (BCI)
- Reads electrical activity in brain (EEG)
- Still largely experimental
- Applications: accessibility, medical

---

## 8. SCREEN DESIGN PRINCIPLES

### Layout and Organization
- **Grouping** – related items together (Gestalt: proximity, similarity)
- **Alignment** – visual consistency
- **White space** – breathing room, reduces clutter
- **Consistency** – uniform appearance throughout

### Text Display
- **Font choice** – sans-serif for screens, serif for print
- **Font size** – minimum 12pt for readability
- **Line length** – 50-75 characters optimal
- **Line spacing** – 1.2-1.5× font size
- **Contrast** – high contrast for readability

### Information Density
- Balance between completeness and clutter
- Progressive disclosure – show detail on demand
- Use of tabs, expandable sections

---

## KEY CONCEPTS FOR EXAM
1. **Display resolution**: pixels (horizontal × vertical), colour depth (bits per pixel)
2. **Colour models**: RGB (additive, displays), HSB (intuitive), CMYK (subtractive, printing)
3. **Colour blindness**: 8% males, 1% females – don't rely on colour alone
4. **Fitts' Law**: applied to pointing devices – large targets, short distances
5. **Mouse**: relative positioning, mechanical/optical/laser
6. **Trackball**: stationary version of mouse
7. **Touchpad**: senses finger position, common on laptops
8. **Joystick**: 2D/3D control, good for gaming/CAD
9. **Pen/Stylus**: direct input, natural writing/drawing
10. **QWERTY**: designed to prevent jamming, not optimized for speed
11. **Audio output**: speech synthesis, earcons, auditory icons
12. **Haptic output**: vibration, force feedback, texture simulation
13. **Speech recognition**: speaker-dependent vs independent, discrete vs continuous
14. **Screen design**: grouping, alignment, white space, consistency
15. **Text display**: sans-serif for screens, 50-75 char line length, high contrast
