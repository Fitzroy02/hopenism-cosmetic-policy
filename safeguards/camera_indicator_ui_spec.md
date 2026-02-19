# CAMERA & MICROPHONE INDICATOR — UI SPEC

## 1. Indicator Requirements
The app must display a **persistent, visible indicator** whenever:

- the camera is active
- the microphone is active
- two-way communication is enabled

---

## 2. Indicator Design
- **Icon:** camera symbol (white on red background)
- **Label:** "Camera Active"
- **Position:** top-right corner
- **Behaviour:**
  - cannot be dismissed
  - remains visible for the entire duration
  - tapping it opens privacy settings

---

## 3. Microphone Variant
- **Icon:** microphone symbol
- **Label:** "Microphone Active"

---

## 4. Combined State
If both are active:

> "Camera & Microphone Active"

---

## 5. Accessibility
- high-contrast mode
- screen-reader announcement
- haptic confirmation on activation
