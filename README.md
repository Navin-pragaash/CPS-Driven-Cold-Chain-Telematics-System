# Projects


Voice streaming embedded system  
Sender: esp32 
Receiver: bluetooth speaker

1. Using a digital microphone simplifies ADC but still requires RTOS for real-time tasks like buffering, processing, and transmitting data.  
2. Total delay includes sampling, processing, buffering, and transmission delays.  
3. Sampling Delay: Depends on sampling rate and buffer size (e.g., 64 ms for 1024 samples at 16 kHz).  
4. Processing Delay: Depends on algorithm complexity, e.g., FFT may take 5-10 ms on ESP32.  
5. Buffering Delay: A ring buffer holding 2048 samples at 16 kHz adds 128 ms delay.  
6. Transmission Delay: Varies by protocol (e.g., Bluetooth ~20 ms, LoRa ~100 ms or more).  
7. Total delay: For a typical system, ~200 ms, which is acceptable for real-time voice streaming.  
8. Optimization: Reduce buffer size, use efficient algorithms, and leverage dual-core ESP32 for parallel tasks.   
10. Properly tuned, ESP32 can achieve <250 ms delay, suitable for voice applications.  





