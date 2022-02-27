
# Design of RF Mixer Circuit Using 28 nm CMOS Technology
# Abstract
Frequency translation which converts the original signal to a much lower baseband frequency signal is a vital role in the RF receiver design. In this work, a down-conversion Gilbert cell mixer is designed using 28 nm RF CMOS process. The mixer covers the frequency band of 3.1-9.5 GHz. The RF mixer provides the high conversion gain with low noise figure at 100MHz IF.
# Introduction
Federal Communication Commission introduced Ultra Wide-Band technology in the frequency range of 3.1-10.6 GHz for unlicensed use. The down conversion mixer is an important component in RF receiver front-end which is shown in Figure 1. The mixer is used as a frequency translation device which down converts the Radio Frequency (RF) signal passing through Low Noise Amplifier (LNA) into Intermediate Frequency (IF) signal. The CMOS technology is used to implement it. The RF parameters such as conversion gain, noise figure and power consumption are important for mixer design. 

**RF Receiver Frontend**

![RFReceiverFrontEnd](https://user-images.githubusercontent.com/100500154/155879861-6ad5b6bc-9b5c-4712-83c2-bdfa78aff0ef.png)

Mixers are used for frequency translation i.e. they are used to convert the RF signal (incoming signal after it is amplified by the LNA) to an intermediate frequency (IF) by multiplying it with a local oscillator (LO) signal. The block level representation is shown in Figure 2. The intermediate frequency can be the sum of frequencies of the two input signals or can be the difference between the two signal frequencies.

**Block Diagram of Mixer**

![BlockLevel](https://user-images.githubusercontent.com/100500154/155879997-e8f3a30d-d25a-4438-a424-0ecb563290b6.png)

# Tool Used
Compiler: Synopsys Custom Compiler

PDK: Synopsys 28 nm CMOS Technology

# Design of RF Mixer Circuit
The conventional Gilbert cell mixer shown in Figure 3 consists of three stages such as Transconductance stage, Mixing stage and Load stage. The RF input signal is given to transconductance stage acting in saturation region where the RF voltage is converted into RF current. The mixing stage is acting in triode region that performs switching by LO signal. 

 **Reference Circuit**
 
 ![Reference](https://user-images.githubusercontent.com/100500154/155880075-b581207b-e73e-4721-8e96-152032c4b81a.png)


 
 **Schematic Diagram**
 
 ![RFMixer](https://user-images.githubusercontent.com/100500154/155879389-f4af6c42-bc8a-48f4-8c58-42f31d6af8e8.png)
 
 
 **Primewave Setup**
 
 ![Testbench](https://user-images.githubusercontent.com/100500154/155879545-bb48c477-28a0-470f-99a5-f3bc4c9d7663.png)

  **Analysis Setup**
  
 ![AnalysisWindow](https://user-images.githubusercontent.com/100500154/155879450-7b08ca49-95ea-4341-8c0b-534e63d607a3.png)

 **Testbench Waveform**
 
 ![Output_Transient](https://user-images.githubusercontent.com/100500154/155879465-9c808447-e681-4284-b141-f3c262ce87af.png)


# Acknowledgement
* Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.
* https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/Synopsys India
* VSD VLSI System Design
* Chinmay panda, IIT Hyderabad
* Sameer Durgoji, NIT Karnataka

# Reference
[1]	First report and order, revision of Part 15 of the commission’s rules regarding ultra wideband transmission systems,  FCC, Washington, DC DC ET Docket, 98-153,2002.

[2]	Behzad R. (2012). RF Microelectronics (2nd ed.). Prentice Hall: Englewood Cliffs. 

[3]	Han, G., & Sanchez-Sinencio, E. (1998). CMOS transconductance multipliers: A tutorial. IEEE Transactions on Circuits and Systems II: Analog and Digital Signal Processing, 45(12), 1550–1563. 

[4]	Kan, K., Ma, D., & Luong, H. (2000). Design theory and performance of 1-GHz CMOS downconversion and upconversion mixers. Analog Integrated Circuits and Signal Processing, 24(2), 101–111
