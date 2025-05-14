IPv4 contains 32 bits and The IPv6 
## IP Address Classes

| Class | First Octet Range | Default Subnet Mask | Network Bits | Host Bits | Hosts per Network |
|-------|-------------------|---------------------|--------------|-----------|--------------------|
| A     | 1 - 126           | 255.0.0.0 (/8)      | 8            | 24        | 16,777,214         |
| B     | 128 - 191         | 255.255.0.0 (/16)   | 16           | 16        | 65,534             |
| C     | 192 - 223         | 255.255.255.0 (/24) | 24           | 8         | 254                |
| D     | 224 - 239         | N/A (Multicast)     | N/A          | N/A       | N/A                |
| E     | 240 - 254         | N/A (Experimental)  | N/A          | N/A       | N/A                |

---

## Subnet Masking Guide

To create subnets, you **borrow bits** from the host part of the IP:

- **Formulae**:
  - Subnets = 2^borrowed_bits
  - Hosts per Subnet = 2^host_bits - 2 (network + broadcast)

### Example - Class C:
- Default: `255.255.255.0` → /24
- Borrow 2 bits → /26 → `255.255.255.192`
- Subnets: `2^2 = 4`
- Hosts per Subnet: `2^6 - 2 = 62`

