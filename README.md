# stm32projectproposal
##  SEEL 5123 (Advanced Microprocessor) Project Proposal. 
### Group members: 
1. Mohamed Afifi Ahmed Mahmoud Khalil  
2. Mahmoud Abdelwase Mahmoud  
3. Omar Amgad elsayed abdelmonem  

## Project Concept and Use Case
This project aims to create a prototype of a robotic dog leg that can be controlled via voice commands. The leg will serve as a building block for a larger project involving the development of a full robot dog. The robotic leg will be controlled by an STM32F4 microcontroller using an on-board microphone and I2S/DMA to process voice commands. Two servos on the robotic leg will be controlled via an I2C servo driver.

To recognize voice commands, the project will use a TensorFlow Lite model, implemented with the help of the STM32_AI_AudioProcessing library and X-CUBE AI. The STM32_AI_AudioProcessing library will provide functions for processing the audio data, while X-CUBE AI will allow for the integration of the TensorFlow Lite model into the STM32F4 microcontroller.

The project will also leverage the CMSIS-DSP and PDMTOPCM libraries to preprocess the audio data before feeding it to the TensorFlow Lite model. A short video will be recorded to demonstrate the functionality of the robotic leg, which will respond to three basic commands: "go", "up", and "down". This project will serve as a proof-of-concept for the larger project of building a full robot dog that can be controlled via voice commands.

## Related Work
[This repository](https://github.com/FedericaPaoli1/stm32-speech-recognition-and-traduction) is the main inspiration and reference for this project. The project uses the above mentioned STM32 libraries to control the on-board LEDs' states by voice. This project extends this idea into the usage of voice to control a robot dog to be much like a real pet dog. The robot leg prototype used is built by a friend, the parts of the program involved with controlling the robot itself is fully custom and not in reference to any other repository. 

## system prelimeinary architecture
[system architecture](sys_arch.jpg)
