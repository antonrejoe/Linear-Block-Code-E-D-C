# Error Correction Coding Simulation with Hamming Code

This project simulates the encoding, transmission, and decoding of messages using Hamming (7,4) code. It includes the addition of Additive White Gaussian Noise (AWGN) to simulate real-world channel conditions and evaluates the performance of error correction techniques.

## Project Overview

The simulation covers:
1. **Message Generation**: Creating randomized binary messages.
2. **Encoding**: Using a generator matrix to encode messages into codewords.
3. **Modulation**: Converting binary codewords into BPSK symbols.
4. **Noise Addition**: Introducing AWGN to simulate channel noise.
5. **Detection & Decoding**: Recovering the original message from noisy signals.
6. **Error Correction**: Using syndromes to detect and correct errors.
7. **Performance Analysis**: Comparing error rates before and after error correction across different SNR levels.

## Key Features

- **Hamming (7,4) Code**: Implements a systematic code capable of correcting single-bit errors.
- **AWGN Channel**: Simulates noisy communication channels with adjustable SNR.
- **Error Correction**: Corrects errors using syndrome decoding.
- **Visualization**: Plots error rates vs. SNR to analyze performance.

## Code Structure

1. **Generator Matrix Creation**:  
   - `create_generator_matrix()`: Constructs the Hamming (7,4) generator matrix.  
2. **Encoding & Modulation**:  
   - `encode_message()`: Encodes messages into codewords.  
   - `modulation()`: Converts bits to BPSK symbols.  
3. **Noise & Decoding**:  
   - `add_awgn()`: Adds Gaussian noise to the signal.  
   - `detect_message()`: Detects symbols from noisy signals.  
   - `decode_msg_all()`: Converts symbols back to bits.  
4. **Error Correction**:  
   - `parity_check_matrix_H()`: Computes the parity-check matrix.  
   - `perform_EC()`: Corrects errors using syndromes.  
5. **Performance Evaluation**:  
   - `perform_info()`: Calculates error rates without correction.  
   - `perform_after_ec()`: Evaluates error rates post-correction.  

## Dependencies

- Python 3.x
- NumPy
- Matplotlib
- Seaborn


