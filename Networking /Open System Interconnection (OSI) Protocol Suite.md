The **Open System Interconnection (OSI)** model structures network communication into **seven layers**, each handling a distinct task. Data flows from the top layer down at the sender and back up at the receiver.
## Key Concepts
- **Layered Architecture**: 
  - Breaks communication into 7 independent layers.
  - Each layer communicates only with adjacent layers via standardized interfaces.
- **Data Flow**:
  - Sender: Data starts at the [[Application Layer]], moves down to the [[Physical Layer]], with headers added at each layer.
  - Receiver: Data ascends from [[Physical Layer]] to [[Application Layer]].
- **Peer-to-Peer Communication**: Both systems initiate and receive data, following the same layered process.
- **Headers**: Each layer appends info for its peer on the remote system (e.g., routing, handling instructions).

## The Seven Layers
1. **[[Application Layer]]**: User interface and application services.
2. **[[Presentation Layer]]**: Data translation, encryption, compression.
3. **[[Session Layer]]**: Manages sessions between applications.
4. **[[Transport Layer]]**: Reliable data transfer (e.g., TCP).
5. **[[Network Layer]]**: Routing and logical addressing (e.g., IP).
6. **[[Data Link Layer]]**: Error-free transfer over physical media.
7. **[[Physical Layer]]**: Hardware and signal transmission.

## Historical Context
- **Goal**: A universal standard for all network models.
- **Outcome**: Too complex and late to market, it failed to replace proprietary models (e.g., TCP/IP).
- **Impact**: Limited interoperability across networks.

## Related
- [[TCP/IP Model]] - A simpler, widely adopted alternative.
- [[Network Protocols]] - Specific rules for each layer.

## OSI Model: Layers, Peer Communication, and Datagrams

The **Open System Interconnection (OSI)** model organizes network communication into **seven layers**. Below are details from the provided tables and figure, formatted for easy reference and linking in Obsidian.

## OSI Protocol Layers and Services (Table 1.1)
The OSI model consists of seven layers, each providing specific services:

- **[[Application Layer]] (7)**: User interface and application-level services.
- **[[Presentation Layer]] (6)**: Data translation, encryption, compression.
- **[[Session Layer]] (5)**: Manages sessions between applications.
- **[[Transport Layer]] (4)**: Ensures reliable data transfer (e.g., segmentation, reassembly).
- **[[Network Layer]] (3)**: Handles routing and logical addressing (e.g., IP).
- **[[Data Link Layer]] (2)**: Ensures error-free transfer over physical media (e.g., framing, error detection).
- **[[Physical Layer]] (1)**: Manages hardware and signal transmission (e.g., cables, bits).

## Logical Peer Communication Model (Figure 1.17)
- **Diagram Description**: Shows peer-to-peer communication between **Machine A** and **Machine B** using the OSI model.
- **Flow**:
  - Data originates at the [[Application Layer]] of Machine A, moves down through each layer (adding headers), and is sent via the [[Physical Layer]] over a channel to Machine B.
  - At Machine B, data ascends from the [[Physical Layer]] back up to the [[Application Layer]], with each layer processing its corresponding peer’s headers.
- **Structure**:
  - Each machine has the same seven layers: [[Application Layer]], [[Presentation Layer]], [[Session Layer]], [[Transport Layer]], [[Network Layer]], [[Data Link Layer]], [[Physical Layer]].
  - Layers communicate only with their peers across machines via standardized interfaces.

## OSI Datagrams with Headers (Table 1.2)
As data moves through the OSI layers, headers are added at each layer. The table shows the datagram structure:

| Layer              | Header | Data         |
|-------------------|--------|--------------|
| [[Application Layer]] | H7     | Data         |
| [[Presentation Layer]] | H6     | Data         |
| [[Session Layer]]    | H5     | Data         |
| [[Transport Layer]]  | H4     | Data         |
| [[Network Layer]]    | H3     | Data         |
| [[Data Link Layer]]  | H2     | Data         |
| [[Physical Layer]]   | No header | Data (Bits) |

- **Process**: 
  - Data starts with no headers at the [[Application Layer]].
  - Each layer adds a header (H7 to H2) as data descends, growing the datagram.
  - The [[Physical Layer]] transmits raw bits without a header.
  - At the receiver, headers are stripped off as data ascends, enabling peer-layer processing.

## Related
- [[OSI Model]] - Overview of the seven-layer model.
- [[Network Protocols]] - Protocols operating at each layer.
- [[TCP/IP Model]] - A simpler, widely used alternative to OSI.

## Notes
- Headers contain control information for peer layers (e.g., routing, error handling).
- The OSI model’s complexity and late adoption limited its replacement of proprietary models like TCP/IP.