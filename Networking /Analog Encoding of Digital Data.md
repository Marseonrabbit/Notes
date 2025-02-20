`Digital data is made up of **1s and 0s** . To send this data over an **analog medium** like a telephone line, we need to convert it into an analog signal. This process is called **modulation** , and the device that does this is called a **modem** (modulator-demodulator).

### 1. **Carrier Signal**
---
- A **carrier signal** is a continuous wave (usually a sine wave) that acts as the base for transmitting data.
- The carrier signal has three main properties that can be changed to encode digital data:
    - **Amplitude** : The height of the wave.
    - **Frequency** : How fast the wave oscillates.
    - **Phase** : The position or timing of the wave.

By changing one or more of these properties, we can represent binary data (1s and 0s).

### 2. **Modulation Techniques**
---
		There xare three common ways to encode digital data into analog signals:

#### **(a) Amplitude Modulation (AM)**

- **How it works** : The amplitude (height) of the carrier wave is changed to represent 1s and 0s.
    - For example:
        - A **low amplitude** (or no wave) could represent a **0** .
        - A **high amplitude** could represent a **1** .
- **Pros and Cons** :
    - Simple but inefficient.
    - Works well only at low speeds (up to **1200 bits per second** ).
    - Not very reliable because noise (interference) can easily affect the signal.

---

#### **(b) Frequency Modulation (FM)**

- **How it works** : The frequency (how fast the wave oscillates) is changed to represent 1s and 0s.
    - For example:
        - A **higher frequency** could represent a **1** .
        - A **lower frequency** could represent a **0** .
- **Pros and Cons** :
    - More reliable than amplitude modulation because it’s less affected by noise.
    - Can handle slightly higher speeds than AM.

---

#### **(c) Phase Shift Modulation (PSM)**

- **How it works** : The phase (timing) of the wave is shifted to represent 1s and 0s.
    - For example:
        - A **180-degree phase shift** could represent a **1** .
        - **No phase shift** could represent a **0** .
- **Pros and Cons** :
    - The most efficient method of the three.
    - Can transmit data at much higher speeds (up to **9600 bits per second** ).
    - Less prone to errors compared to AM and FM.

### 3. **Why Use Modems?**

- A **modem** converts digital data from your computer into analog signals that can travel over phone lines (modulation).
- At the receiving end, the modem converts the analog signal back into digital data (demodulation).

---

### Summary

- **Digital data (1s and 0s)** needs to be converted into **analog signals** to travel over analog media like phone lines.
- This is done using **modulation techniques** :
    1. **Amplitude Modulation (AM)** : Changes wave height (inefficient, slow).
    2. **Frequency Modulation (FM)** : Changes wave frequency (more reliable).
    3. **Phase Shift Modulation (PSM)** : Changes wave timing (most efficient, faster).
- A **modem** handles the conversion between digital and analog signals.

This is how computers send data over old-school phone lines!
