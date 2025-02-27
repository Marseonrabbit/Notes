## 1. Transmission Technology
Core function: Propagation/processing of signals between network elements using encoding schemes to convert data into analog/digital signals.

### 1.1 Analog Encoding of Digital Data
**Purpose**: Transmit digital data over analog media (e.g., telephone lines)  
**Modulation Techniques**:  
- **Amplitude Modulation (AM)**  
  - Represents bits via amplitude changes (0=low amplitude, 1=high amplitude)  
  - Limited to **1200 bps** due to noise susceptibility  
  - Uses sine wave carrier signals (voice-grade lines)  
  - Example: Early dial-up modems  

- **Frequency Modulation (FM)**  
  - Encodes 1s as high-frequency waves (1070/1270 Hz), 0s as low-frequency waves  
  - Error-resistant design (Bell 202 standard)  
  - Achieves **up to 2400 bps**  

- **Phase Shift Modulation (PSK)**  
  - Encodes 1s as 180° phase shifts, 0s as no shift  
  - Highest efficiency (**9600 bps** via V.22bis standard)  
  - Used in modern DSL technologies  

**Hardware**: Requires modems (modulator-demodulator pairs)  
**Limitations**:  
- Bandwidth constraints of analog media  
- Signal degradation over distance  

---

### 1.2 Digital Encoding of Digital Data
**Implementation**: Voltage pulses (e.g., 0V=0, 5V=1)  
**Key Schemes**:  
- **NRZ-L**  
  - Negative voltage = 1, Positive voltage = 0  
  - Requires precise clock synchronization  
  - Used in RS-232 serial communication  
![[Pasted image 20250227171152.png]]
- **NRZ-I**  
  - Encodes 1s as voltage transitions, 0s as no change  
  - Reduces baseline drift issues  
  - Found in USB 2.0 protocols  
![[Pasted image 20250227171207.png]]
- **Manchester Encoding**  
  - Combines clock + data signals (transition at midpoint of each bit)  
  - Used in **Ethernet (10BASE-T)** and IEEE 802.3 standards  
  - Self-clocking at **10 Mbps**  

- **Differential Manchester**  
  - Transition at start of bit = 0, no transition = 1  
  - Better noise immunity (used in Token Ring networks)  

**Advantages Over Analog**:  
1. **Cost**: Digital circuits 70% cheaper than analog equivalents  
2. **Integration**: Supports voice/video/text convergence (VoIP, IPTV)  
3. **Signal Integrity**: Repeaters every 2-5 km vs amplifiers every 1 km  
4. **Security**: AES-256 encryption vs analog scrambling  
5. **Bandwidth Efficiency**: 40% better spectral efficiency  

---

### 1.3 Multiplexing Techniques
**Purpose**: Maximize medium utilization through signal sharing  
**Types**:  
- **FDM (Frequency-Division)**  
  - Analog signals modulated to 4 kHz channels (telephony standard)  
  - Full-duplex support via guard bands  
  - Example: Cable TV (6 MHz channels)  

- **TDM (Time-Division)**  
  - **Synchronous TDM**: Fixed time slots (T1/E1 lines - 24/30 channels)  
  - **Statistical TDM**: Dynamic slot allocation (802.11 Wi-Fi)  
  - Requires <10 ppm clock synchronization  

---

## 2. Transmission Media

### 2.1 Wired Media
**Twisted Pair (ANSI/TIA-568)**  
- **Structure**: 4 twisted pairs (Cat5e: 100 MHz, Cat6: 250 MHz)  
- **Performance**:  
  - **Cat3**: 10 Mbps (voice-grade)  
  - **Cat5e**: 1 Gbps up to 100m  
  - **Cat6A**: 10 Gbps up to 100m  
- **Shielding**: UTP (unshielded) vs STP (foil shielded)  
![[Pasted image 20250227171334.png]]
**Coaxial Cable (IEEE 802.3)**  
- **Thinnet (RG-58)**:  
  - 5 mm diameter, 10 Mbps up to 185m  
  - Used in legacy Ethernet (10BASE2)  
- **Thicknet (RG-8)**:  
  - 10 mm diameter, 10 Mbps up to 500m  
  - Backbone networks (10BASE5)  

**Fiber Optics (ITU-T G.652)**  
- **Core**: 8-10 µm (single-mode), 50-62.5 µm (multi-mode)  
- **Performance**:  
  - **OM4 Multi-mode**: 100 Gbps up to 150m  
  - **OS2 Single-mode**: 100 Gbps up to 10 km  
- **Connectors**: LC, SC, MTP® (85% market share)  
![[Pasted image 20250227171317.png]]
---

### 2.2 Wireless Media
**Infrared (IrDA)**  
- **850-900 nm wavelength**  
- **Speed**: 16 Mbps (IrDA 1.1)  
- **Use Case**: Medical devices (EMI-sensitive environments)  

**Radio Frequency (IEEE 802.11)**  
- **2.4 GHz ISM Band**:  
  - 14 channels (22 MHz spacing)  
  - 802.11g: 54 Mbps  
- **5 GHz UNII Band**:  
  - 23 non-overlapping channels  
  - 802.11ac: 1.3 Gbps (MU-MIMO)  

**Microwave**  
- **Terrestrial**:  
  - 6-42 GHz bands  
  - **E-band (70-80 GHz)**: 10 Gbps links  
  - Tower spacing: 30-50 km  
- **Satellite**:  
  - **C-band (4-8 GHz)**: 500 Mbps (VSAT)  
  - **Ka-band (26.5-40 GHz)**: 100 Gbps (HTS)  

**Laser (FSO)**  
- **850 nm wavelength**  
- **Speed**: 10 Gbps (1 km range)  
- **Use Case**: Metro network backhaul  

---

## 3. Network Performance Factors
| Parameter       | Twisted Pair       | Coaxial          | Fiber Optic      | Wireless         |
|-----------------|-------------------|------------------|------------------|------------------|
| **Bandwidth**   | 10 Gbps (Cat6A)   | 1 Gbps           | 100 Tbps         | 10 Gbps (Wi-Fi6) |
| **Distance**    | 100m              | 500m             | 100 km           | 100m (indoor)    |
| **Attenuation** | 20 dB/km          | 8 dB/km          | 0.2 dB/km        | 30 dB (2.4 GHz)  |
| **Latency**     | 0.01 ms/km        | 0.005 ms/km      | 0.004 ms/km      | 1-100 ms         |
| **Cost**        | $0.1/m            | $0.5/m           | $1.5/m           | $0.05/m (RF)     |

**Key Considerations**:  
- **EMI Resistance**: Fiber > Coaxial > Twisted Pair  
- **Security**: Fiber (NSA-certified) > Coaxial > Wireless  
- **Installation**: Wireless < Twisted Pair < Coaxial << Fiber  

[[Network Topology]] [[Modulation Techniques]] [[Network Topology]] [[IEEE Standards]]