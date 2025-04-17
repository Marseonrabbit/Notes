| Feature         | TCP (Transmission Control Protocol)   | UDP (User Datagram Protocol)       |
| --------------- | ------------------------------------- | ---------------------------------- |
| Connection      | Connection-oriented                   | Connectionless                     |
| Reliability     | Reliable (guarantees delivery, order) | Unreliable (no delivery guarantee) |
| Speed           | Slower due to overhead                | Faster (less overhead)             |
| Use Cases       | Web browsing, email, file transfer    | Video streaming, gaming, VoIP      |
| Header Size     | Larger                                | Smaller                            |
| Packet Delivery | Ordered and acknowledged              | No ordering, no acknowledgment     |

Client                             Server
  |                                  |
  | ----------- SYN ------------>    |  (Step 1)
  |                                  |
  | <-------- SYN-ACK ----------     |  (Step 2)
  |                                  |
  | ----------- ACK ------------>    |  (Step 3)
  |                                  |

 Connection Established!
