# Chapter 2: The Computer — The Other Half of the Dialogue

## The Big Picture

Chapter 1 covered the **human** side of the interaction. Chapter 2 covers the **computer** side — the devices that output information to the user and take input from them. If Chapter 1 asked "what are humans capable of?", this chapter asks "what can the computer do to meet them halfway?"

Think of the computer's I/O as a mirror to human I/O:

| Human | Computer |
|-------|----------|
| Vision | Displays (text, graphics, colour, audio, haptic) |
| Movement/Speech/Gesture | Input devices (keyboard, mouse, touch, speech, eye tracking) |

---

## 1. OUTPUT — How the Computer Speaks to the User

### Displays — The Primary Output Channel

**Display technologies** have evolved from CRT (electron beam on phosphors) to flat panels (LCD, plasma, OLED). Three key specs define a display:

- **Resolution** — pixels (horizontal × vertical)
- **Colour depth** — bits per pixel (1-bit = B&W, 8-bit = 256 colours, 24-bit = true colour)
- **Refresh rate** — how often the image redraws (too low → flicker)

Other characteristics: **luminance** (brightness), **contrast** (difference between brightest white and darkest black), **gamma** (nonlinear relationship between pixel value and actual brightness).

#### Text Displays vs. Graphics Displays

| | Text Display | Graphics Display |
|--|-------------|-----------------|
| How it works | Characters from a fixed matrix (e.g., 5×7 dots) | Each pixel individually addressable |
| Pros | Fast to render, simple | Arbitrary shapes, fonts, images |
| Cons | Limited character set, limited typography | More memory and processing needed |
| Enhancement | — | **Anti-aliasing** smooths jagged edges |

### Audio Output — The Secondary Channel

Three types of computer-generated sound:

1. **Speech synthesis** — text-to-speech (slow but attention-getting)
2. **Earcons** — musical sounds that represent actions/objects
3. **Auditory icons** — real-world sounds (e.g., crumpling paper for "delete")

**Uses**: accessibility (visually impaired), alerts, navigation feedback, entertainment. Non-speech audio is faster than speech. Cultural differences in interpretation matter.

### Haptic Output — Touch Feedback

Three types:

1. **Vibration** — tactile alerts (phones)
2. **Force feedback** — resistance to movement (game controllers)
3. **Texture simulation** — surface roughness

**Uses**: mobile alerts, gaming, surgical simulation, accessibility.

---

## 2. INPUT — How the User Speaks to the Computer

### Keyboards — The Text Workhorse

Most common input device. Standard layout is **QWERTY** (designed to prevent mechanical jamming, not for speed). Alternatives: **Dvorak** (optimized for efficiency), **chord keyboards** (multiple keys at once), **soft keyboards** (on-screen for touch/pen).

### Pointing Devices

| Device | How It Works | Best For | Downside |
|--------|-------------|----------|----------|
| **Mouse** | Measures relative movement (mechanical/optical/laser) | Direct manipulation | Needs flat surface, one-handed |
| **Trackball** | Stationary, ball on top moved by fingers | Compact spaces | Less precise than mouse |
| **Touchpad** | Senses finger position | Laptops (no moving parts) | Small area, less precise |
| **Joystick** | Lever controls position/direction | Gaming, CAD, simulation | Fatigue, imprecise for text |
| **Pen/Stylus** | Direct input on screen | Drawing, writing, tablets | Occlusion (hand blocks view), fatigue |

### Other Input Modalities

**Speech Recognition** — converts spoken words to text/commands. Two dimensions:
- Speaker-dependent (trained) vs. speaker-independent (any voice)
- Discrete (word by word) vs. continuous (natural speech)

Challenges: noise, accents, vocabulary size, accuracy.

**Gesture Recognition** — detects body movements via cameras, gloves, or accelerometers. Used for sign language, gaming, VR.

**Eye Tracking** — tracks eye position and movement. Measures **fixations** (where you pause), **saccades** (rapid jumps), and **scan paths** (the overall pattern). Used for accessibility, research, advertising.

**Brain-Computer Interface (BCI)** — reads EEG brain activity. Still largely experimental. Used for accessibility and medical applications.

---

## 3. COLOUR — A Critical Bridge Between Human and Computer

### Colour Models

Different models serve different purposes:

| Model | How It Works | Used For |
|-------|-------------|----------|
| **RGB** (Red, Green, Blue) | Additive — combines light | Displays (0-255 per channel, 24-bit = 16.7M colours) |
| **HSB/HSV** (Hue Saturation Brightness) | Intuitive for humans | Design tools |
| **CMYK** (Cyan Magenta Yellow Key) | Subtractive — absorbs light | Printing |

### Colour in Interface Design

- **Red** → warning, error, stop
- **Green** → okay, go, success
- **Blue** → information, links

**Critical rules**:
- Use colour meaningfully and consistently
- Don't rely on colour alone — **8% of men and 1% of women are colour blind**
- Use redundant cues (shapes, patterns, text labels)

### Display Colour Issues

- **Gamma correction** — compensates for the nonlinear relationship between pixel value and screen brightness
- **Colour calibration** — ensures consistency across devices
- **Metamerism** — different spectral compositions can appear as the same colour

---

## 4. SCREEN DESIGN PRINCIPLES — Putting It All Together

### Layout & Organization

Four principles borrowed from Gestalt psychology:
1. **Grouping** — related items together (proximity, similarity)
2. **Alignment** — visual consistency throughout
3. **White space** — breathing room reduces clutter
4. **Consistency** — uniform appearance

### Text Display Rules

| Rule | Guideline |
|------|-----------|
| Font choice | Sans-serif for screens, serif for print |
| Font size | Minimum 12pt for readability |
| Line length | 50-75 characters optimal |
| Line spacing | 1.2–1.5× font size |
| Contrast | High contrast essential |

### Information Density

Balance completeness vs. clutter. Use **progressive disclosure** — show detail on demand via tabs, expandable sections, etc.

---

## KEY CONCEPTS FOR EXAM

1. **Display specs**: resolution (pixels), colour depth (bits/pixel), refresh rate
2. **Colour models**: RGB (additive, displays), HSB (intuitive), CMYK (subtractive, printing)
3. **Colour blindness**: 8% males, 1% females — never rely on colour alone
4. **Fitts' Law applied**: large targets, short distances
5. **Mouse**: relative positioning, mechanical/optical/laser
6. **Trackball**: stationary mouse, good for limited space
7. **Touchpad**: finger position sensing, laptop standard
8. **Joystick**: 2D/3D control, gaming/CAD
9. **Pen/Stylus**: direct input, natural writing, occlusion problem
10. **QWERTY**: anti-jam design, not speed-optimized
11. **Audio output**: speech synthesis, earcons, auditory icons
12. **Haptic output**: vibration, force feedback, texture
13. **Speech recognition**: speaker-dependent vs independent; discrete vs continuous
14. **Screen design**: grouping, alignment, white space, consistency
15. **Text display**: sans-serif for screens, 50-75 char lines, high contrast
