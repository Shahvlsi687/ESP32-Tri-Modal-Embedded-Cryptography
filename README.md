# ESP32-Based Tri-Modal Embedded Cryptography Framework with Position-Variant PVRSC

## 📝 Project Overview
Engineered an embedded C++ cipher framework on an ESP32 SoC, integrating a custom Position-Variant Radial Stick Cipher (PVRSC) for resource-constrained edge nodes. Neutralized visual frequency analysis by executing on-chip, index-dependent geometric transformations that map characters to unique vector orientations on an SSD1306 OLED framebuffer via a fast-mode 400 kHz I2C pipeline.

## 🧱 Core Algorithmic Architecture
The firmware operates as an independent, zero-dependency sub-system utilizing pure C++ integer-based arithmetic to achieve optimal performance metrics on low-power edge nodes:

1. **Position-Variant Radial Stick Cipher (PVRSC):** Translates printable ASCII character streams into discrete on-chip geometric vector lines radiating from a central coordinate. By incorporating character indices into the sector angle formula, identical characters yield completely different visual quadrant configurations, eliminating shoulder-surfing frequency leaks.
2. **Magic Square Zigzag Cipher (MSZC):** Dynamically constructs odd-order Siamese magic squares matching incoming string dimensions. Implements a double-stage transposition using alternating left-to-right and right-to-left zigzag matrix readings to break sequential data structures entirely through integer operations.
3. **Fractal Substitution Cipher (FSC):** A multi-level, polyalphabetic substitution engine executing recursive range-splitting and reversal mapping on character sets to mask highly repetitive sensor data streams.

---

## 📊 Verification & Visual Metrics

### 1. Cryptographic Execution Metrics
Below is the verification capture from the serial debugging console showing the computational metrics, entropy stability, and execution footprints:

<!-- REPLACE THE LINK BELOW WITH YOUR METRICS SCREENSHOT -->
![Cryptographic Performance Metrics](screenshots/PLACEHOLDER_FOR_METRICS_IMAGE.png)

### 2. Real-Time Geometric OLED Outputs
The image below displays the abstract, position-variant radial stick arrays rendered directly onto the SSD1306 framebuffer, confirming successful visual obfuscation:

<!-- REPLACE THE LINK BELOW WITH YOUR OLED SCREENSHOT -->
![OLED Framebuffer Render Output](screenshots/PLACEHOLDER_FOR_OLED_IMAGE.png)

---

## 🛠️ Hardware & Environment Stack
* **Processor SoC:** Espressif Systems ESP32-WROOM-32 (Dual-core Xtensa LX6 @ 240 MHz)
* **Display Peripheral:** 128×64 pixels monochrome SSD1306 OLED Controller IC
* **Bus Architecture:** 400 kHz I2C Interface (GPIO 21 SDA / GPIO 22 SCL)
* **Development Platform:** Arduino Core Environment (Pure C++ / math.h)
* **Memory Footprint:** Fully optimized standalone sketch operating under a strict 15 KB program memory space.

---

