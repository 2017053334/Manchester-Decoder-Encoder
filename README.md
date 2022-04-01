# Manchester-Decoder-Encoder
Design a  Manchester Decoder and Encoder
# Manchester Decoder and Encoder 

## Manchester Code Decoder

The schematic of the `Manchester Code Decoder`  is shown as bellowed:

![Manchester](https://github.com/2017053334/Manchester-Decoder-Encoder/blob/master/design%20report/picture/Manchester.png)

The waveform of the `Manchester Code Decoder`  is shown as bellowed:

<img src="https://github.com/2017053334/Manchester-Decoder-Encoder/blob/master/design%20report/picture/waveform .png" alt="waveform " style="zoom:50%;" />

The Manchester bit value is presented in the first half of each bit time. Here we can generate a clock to capture the value at 1/4 bit time.

Function of XOR gate: Provide the start time for the counter.

Function of two AND gate and OR gate: Ensure 1/4 bit time pulse width.

Function of inverter: Flip the signal so that the rising edge appears in 1/4 bit time.

Function of counter and comparator:

- Generate clock.

- Manchester Code data rate is 2Mbps(2000000 bit/s), so  F is equal to 2MHz.

- Frequency of Oscillation is fosc, so 3/4 bit time is equal to <img src="E:\DESKTOP\number.png" alt="number" style="zoom: 50%;" />.

- Set <img src="E:\DESKTOP\number.png" alt="number" style="zoom: 50%;" /> as Counter's Initial number, Counter number compare with <img src="E:\DESKTOP\number.png" alt="number" style="zoom: 50%;" />, output "1" if smaller and output "0" if larger.

  For example: 

  fosc = 8MHz, Initial number = 3, binary number = 11

  ![Counter](E:\DESKTOP\Counter.png)

## Manchester Code Encoder

The schematic of the `Manchester Code Encoder`  is shown as bellowed:

![encoder_schematic](E:\DESKTOP\encoder_schematic.png)

The waveform of the `Manchester Code Encoder`  is shown as bellowed:

<img src="E:\DESKTOP\encoder_waveform.png" alt="encoder_waveform" style="zoom:50%;" />
