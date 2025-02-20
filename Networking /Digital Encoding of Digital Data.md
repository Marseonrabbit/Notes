In **digital encoding** , we send digital data (1s and 0s) as **digital signals** . This is the most common and easiest way to transmit data between devices like computers.

---
### How It Works

- Digital signals use **two voltage levels** to represent binary digits:
    - For example:
        - **0 volts** could mean **0** .
        - **5 volts** could mean **1** .
    - These voltages are easy for computers to understand because they "think" in binary.

---
### Common Encoding Methods

There are different ways to encode digital data into signals. Here are two popular ones:

#### 1. **NRZ-L (Non-Return-to-Zero Level)**

- In this method:
    - A **negative voltage** represents a **1** .
    - A **positive voltage** represents a **0** .
- The signal stays at one voltage level until it needs to change for the next bit.
- **Problem** : If there are long sequences of 1s or 0s, the receiver might lose track of where one bit ends and the next begins. This happens because the clocks of the sender and receiver can get out of sync.
![[Pasted image 20250220192316.png]]
---

#### 2. **NRZ-I (Non-Return-to-Zero, Invert on Ones)**

- In this method:
    - A **1** is represented by a **change in voltage** (either up or down).
    - A **0** means **no change** in voltage.
- This is slightly better than NRZ-L because changes in voltage help the receiver stay in sync.
![[Pasted image 20250220192345.png]]
---

### Better Encoding Methods: Manchester and Differential Manchester

To solve the synchronization problem, other encoding methods like **Manchester** and **Differential Manchester** were developed:

- **Manchester Encoding** :
    
    - Combines the clock signal with the data.
    - A **1** is represented by a voltage transition from high to low in the middle of the bit.
    - A **0** is represented by a voltage transition from low to high in the middle of the bit.
    - This ensures that there’s always a transition, so the receiver can stay in sync.
- **Differential Manchester** :
    
    - Similar to Manchester, but instead of using transitions to represent 1s and 0s, it uses the **presence or absence** of a transition at the start of the bit.
    - A **1** means no transition at the start of the bit.
    - A **0** means there is a transition at the start of the bit.

These methods are more reliable because they include timing information along with the data.

---

### Why Use Digital Encoding?

Digital encoding has several advantages over analog encoding:

1. **Cheaper Technology** : Digital circuits are becoming cheaper and easier to produce.
2. **Better Integration** : It’s easier to combine different types of data (voice, video, text, images) in digital form.
3. **Less Noise** : Digital signals are less affected by noise and interference. Repeaters can clean up the signal as it travels.
4. **Efficient Use of Channels** : Digital techniques make better use of the available bandwidth.
5. **Improved Security** : Digital data can be encrypted, making it more secure than analog signals.

---

### Summary

- **Digital encoding** uses two voltage levels to represent binary data (1s and 0s).
- Common methods include **NRZ-L** , **NRZ-I** , **Manchester** , and **Differential Manchester** .
- **Manchester** and **Differential Manchester** solve synchronization problems by including timing information in the signal.
- **Advantages of digital encoding** :
    - Cheaper and more efficient.
    - Better integration of data types.
    - Less noise and interference.
    - Improved security through encryption.

This is why digital encoding is widely used in modern communication systems!