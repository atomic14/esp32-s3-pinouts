

Testing a ESP32-S3-DevKitC-1 for Pins: 


Mouser-Nr.:356-ESS3DVKTC1N32R8V
Herst.- Nr.: ESP32-S3-DevKitC-1-N32R8V

Testing: 

# Full GPIO Table

- I - input
- O - output
- T - tristate (high impedance)

| Pin Name | Pin Number | Type | Description |
|----------|------------|------|-------------|
| GND      | 1,40       | P    | **GND**         |
| EPAD     | 41         | P    | **GND** |
| 3V3      | 2          | P    | **Power supply**|
| EN       | 3          | I    | High: on, enables the chip. Low: off, the chip powers off. Note: Do not leave the EN pin floating. |
| <span style="color: orange;">GPIO0</span>    | 27         | I/O/T| RTC_GPIO0, **GPIO0** |
| GPIO1    | 39         | I/O/T| RTC_GPIO1, **GPIO1**, TOUCH1, ADC1_CH0 |
| GPIO2    | 38         | I/O/T| RTC_GPIO2, **GPIO2**, TOUCH2, ADC1_CH1 |
| <span style="color: orange;">GPIO3</span>    | 15         | I/O/T| RTC_GPIO3, **GPIO3**, TOUCH3, ADC1_CH2 |
| GPIO4    | 4          | I/O/T| RTC_GPIO4, **GPIO4**, TOUCH4, ADC1_CH3 |
| GPIO5    | 5          | I/O/T| RTC_GPIO5, **GPIO5**, TOUCH5, ADC1_CH4 |
| GPIO6    | 6          | I/O/T| RTC_GPIO6, **GPIO6**, TOUCH6, ADC1_CH5 |
| GPIO7    | 7          | I/O/T| RTC_GPIO7, **GPIO7**, TOUCH7, ADC1_CH6 |
| GPIO8    | 12         | I/O/T| RTC_GPIO8, **GPIO8**, TOUCH8, ADC1_CH7, SUBSPICS1 |
| GPIO9    | 17         | I/O/T| RTC_GPIO9, **GPIO9**, TOUCH9, ADC1_CH8, FSPIHD, SUBSPIHD |
| GPIO10   | 18         | I/O/T| RTC_GPIO10, **GPIO10**, TOUCH10, ADC1_CH9, FSPICS0, FSPIIO4, SUBSPICS0 |
| GPIO11   | 19         | I/O/T| RTC_GPIO11, **GPIO11**, TOUCH11, ADC2_CH0, FSPID, FSPIIO5, SUBSPID |
| GPIO12   | 20         | I/O/T| RTC_GPIO12, **GPIO12**, TOUCH12, ADC2_CH1, FSPICLK, FSPIIO6, SUBSPICLK |
| GPIO13   | 21         | I/O/T| RTC_GPIO13, **GPIO13**, TOUCH13, ADC2_CH2, FSPIQ, FSPIIO7, SUBSPIQ |
| GPIO14   | 22         | I/O/T| RTC_GPIO14, **GPIO14**, TOUCH14, ADC2_CH3, FSPIWP, FSPIDQS, SUBSPIWP |
| GPIO15   | 8          | I/O/T| RTC_GPIO15, **GPIO15**, U0RTS, ADC2_CH4, XTAL_32K_P |
| GPIO16   | 9          | I/O/T| RTC_GPIO16, **GPIO16**, U0CTS, ADC2_CH5, XTAL_32K_N |
| GPIO17   | 10         | I/O/T| RTC_GPIO17, **GPIO17**, U1TXD, ADC2_CH6 |
| GPIO18   | 11         | I/O/T| RTC_GPIO18, **GPIO18**, U1RXD, ADC2_CH7, CLK_OUT3 |
| <span style="color: red;">USB_D-</span>   | 13         | I/O/T| RTC_GPIO19, GPIO19, U1RTS, ADC2_CH8, CLK_OUT2, **USB_D-** |
| <span style="color: red;">USB_D+</span>   | 14         | I/O/T| RTC_GPIO20, GPIO20, U1CTS, ADC2_CH9, CLK_OUT1, **USB_D+** |
| GPIO21   | 23         | I/O/T| RTC_GPIO21, **GPIO21** |
| <span style="color: red;">GPIO35</span>   | 28         | I/O/T| SPIIO6, **GPIO35**, FSPID, SUBSPID |
| <span style="color: red;">GPIO36</span>   | 29         | I/O/T| SPIIO7, **GPIO36**, FSPICLK, SUBSPICLK |
| <span style="color: red;">GPIO37</span>   | 30         | I/O/T| SPIDQS, **GPIO37**, FSPIQ, SUBSPIQ |
| GPIO38   | 31         | I/O/T| **GPIO38**, FSPIWP, SUBSPIWP |
| <span style="color: red;">MTCK</span>   | 32         | I/O/T| **MTCK**, GPIO39, CLK_OUT3, SUBSPICS1 |
| <span style="color: red;">MTDO</span>   | 33         | I/O/T| **MTDO**, GPIO40, CLK_OUT2 |
| <span style="color: red;">MTDI</span>   | 34         | I/O/T| **MTDI**, GPIO41, CLK_OUT1 |
| <span style="color: red;">MTMS</span>   | 35         | I/O/T| **MTMS**, GPIO42 |
| <span style="color: red;">U0TXD</span>   | 37         | I/O/T| **U0TXD**, GPIO43, CLK_OUT1 |
| <span style="color: red;">U0RXD</span>   | 36         | I/O/T| **U0RXD**, GPIO44, CLK_OUT2 |
| <span style="color: orange;">GPIO45</span>   | 26         | I/O/T| **GPIO45** |
| <span style="color: orange;">GPIO46</span>   | 16         | I/O/T| **GPIO46** |
| GPIO47   | 24         | I/O/T| SPICLK_P_DIFF, **GPIO47**, SUBSPICLK_P_DIFF |
| GPIO48   | 25         | I/O/T| SPICLK_N_DIFF, **GPIO48**, SUBSPICLK_N_DIFF |
