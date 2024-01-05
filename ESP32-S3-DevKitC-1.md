

Testing a ESP32-S3-DevKitC-1 for Pins: 


Mouser-Nr.:356-ESS3DVKTC1N32R8V
Herst.- Nr.: ESP32-S3-DevKitC-1-N32R8V

Testing: 

[ESP32-S3-DevKitC-1 v1.1](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s3/hw-reference/esp32s3/user-guide-devkitc-1.html)


Testing with a ["Hello World" Example](https://github.com/diplfranzhoepfinger/esp32-s3-pinouts-tester) 

# Full GPIO Table

- I - input
- O - output
- T - tristate (high impedance)

| Pin Name | Pin Number | Pin Number Devk  | Default Voltage |  Type |                                             Description                                            |
|:--------:|:----------:|-----------------:|-----------------|:-----:|:--------------------------------------------------------------------------------------------------:|
| GND      | 1,40       |                  |                 | P     | **GND**                                                                                            |
| EPAD     | 41         |                  |                 | P     | **GND**                                                                                            |
| 3V3      | 2          |                  |                 | P     | **Power supply**                                                                                   |
| EN       | 3          |                  |                 | I     | High: on, enables the chip. Low: off, the chip powers off. Note: Do not leave the EN pin floating. |
| GPIO0    | 27         | J3-14            | 3.3V            | I/O/T | RTC_GPIO0, **GPIO0**                                                                               |
| GPIO1    | 39         | J3-4             | 0.0V            | I/O/T | RTC_GPIO1, **GPIO1**, TOUCH1, ADC1_CH0                                                             |
| GPIO2    | 38         | J3-5             | 0.0V            | I/O/T | RTC_GPIO2, **GPIO2**, TOUCH2, ADC1_CH1                                                             |
| GPIO3    | 15         | J1-13            | 0.0V            | I/O/T | RTC_GPIO3, **GPIO3**, TOUCH3, ADC1_CH2                                                             |
| GPIO4    | 4          | J1-4             | 0.0V            | I/O/T | RTC_GPIO4, **GPIO4**, TOUCH4, ADC1_CH3                                                             |
| GPIO5    | 5          | J1-5             | 0.0V            | I/O/T | RTC_GPIO5, **GPIO5**, TOUCH5, ADC1_CH4                                                             |
| GPIO6    | 6          | J1-6             | 0.0V            | I/O/T | RTC_GPIO6, **GPIO6**, TOUCH6, ADC1_CH5                                                             |
| GPIO7    | 7          | J1-7             | 0.0V            | I/O/T | RTC_GPIO7, **GPIO7**, TOUCH7, ADC1_CH6                                                             |
| GPIO8    | 12         | J1-12            | 0.0V            | I/O/T | RTC_GPIO8, **GPIO8**, TOUCH8, ADC1_CH7, SUBSPICS1                                                  |
| GPIO9    | 17         | J1-15            | 0.0V            | I/O/T | RTC_GPIO9, **GPIO9**, TOUCH9, ADC1_CH8, FSPIHD, SUBSPIHD                                           |
| GPIO10   | 18         | J1-16            | 0.0V            | I/O/T | RTC_GPIO10, **GPIO10**, TOUCH10, ADC1_CH9, FSPICS0, FSPIIO4, SUBSPICS0                             |
| GPIO11   | 19         | J1-17            | 0.0V            | I/O/T | RTC_GPIO11, **GPIO11**, TOUCH11, ADC2_CH0, FSPID, FSPIIO5, SUBSPID                                 |
| GPIO12   | 20         | J1-18            | 0.0V            | I/O/T | RTC_GPIO12, **GPIO12**, TOUCH12, ADC2_CH1, FSPICLK, FSPIIO6, SUBSPICLK                             |
| GPIO13   | 21         | J1-19            | 0.0V            | I/O/T | RTC_GPIO13, **GPIO13**, TOUCH13, ADC2_CH2, FSPIQ, FSPIIO7, SUBSPIQ                                 |
| GPIO14   | 22         | J1-20            | 0.0V            | I/O/T | RTC_GPIO14, **GPIO14**, TOUCH14, ADC2_CH3, FSPIWP, FSPIDQS, SUBSPIWP                               |
| GPIO15   | 8          | J1-8             | 0.0V            | I/O/T | RTC_GPIO15, **GPIO15**, U0RTS, ADC2_CH4, XTAL_32K_P                                                |
| GPIO16   | 9          | J1-9             | 0.0V            | I/O/T | RTC_GPIO16, **GPIO16**, U0CTS, ADC2_CH5, XTAL_32K_N                                                |
| GPIO17   | 10         | J1-10            | 0.0V            | I/O/T | RTC_GPIO17, **GPIO17**, U1TXD, ADC2_CH6                                                            |
| GPIO18   | 11         | J1-11            | 0.0V            | I/O/T | RTC_GPIO18, **GPIO18**, U1RXD, ADC2_CH7, CLK_OUT3                                                  |
| USB_D-   | 13         | J3-20            | 0.0V            | I/O/T | RTC_GPIO19, GPIO19, U1RTS, ADC2_CH8, CLK_OUT2, **USB_D-**                                          |
| USB_D+   | 14         | J3-19            | 3.3V            | I/O/T | RTC_GPIO20, GPIO20, U1CTS, ADC2_CH9, CLK_OUT1, **USB_D+**                                          |
| GPIO21   | 23         | J3-18            | 0.0V            | I/O/T | RTC_GPIO21, **GPIO21**                                                                             |
| GPIO35   | 28         | J3-13            | 0.0V            | I/O/T | SPIIO6, **GPIO35**, FSPID, SUBSPID                                                                 |
| GPIO36   | 29         | J3-12            | 0.0V            | I/O/T | SPIIO7, **GPIO36**, FSPICLK, SUBSPICLK                                                             |
| GPIO37   | 30         | J3-11            | 0.0V            | I/O/T | SPIDQS, **GPIO37**, FSPIQ, SUBSPIQ                                                                 |
| GPIO38   | 31         | J3-10            | 0.0V            | I/O/T | **GPIO38**, FSPIWP, SUBSPIWP                                                                       |
| MTCK     | 32         | J3-9             | 3.3V            | I/O/T | **MTCK**, GPIO39, CLK_OUT3, SUBSPICS1                                                              |
| MTDO     | 33         | J3-8             | 0.0V            | I/O/T | **MTDO**, GPIO40, CLK_OUT2                                                                         |
| MTDI     | 34         | J3-7             | 0.0V            | I/O/T | **MTDI**, GPIO41, CLK_OUT1                                                                         |
| MTMS     | 35         | J3-6             | 0.0V            | I/O/T | **MTMS**, GPIO42                                                                                   |
| U0TXD    | 37         | J3-2             | 3.3V            | I/O/T | **U0TXD**, GPIO43, CLK_OUT1                                                                        |
| U0RXD    | 36         | J3-3             | 3.3V            | I/O/T | **U0RXD**, GPIO44, CLK_OUT2                                                                        |
| GPIO45   | 26         | J3-15            | 0.0V            | I/O/T | **GPIO45**                                                                                         |
| GPIO46   | 16         | J1-14            | 0.0V            | I/O/T | **GPIO46**                                                                                         |
| GPIO47   | 24         | J3-17            | 0.0V *3.3V      | I/O/T | SPICLK_P_DIFF, **GPIO47**, SUBSPICLK_P_DIFF                                                        |
| GPIO48   | 25         | J3-16            | 0.0V            | I/O/T | SPICLK_N_DIFF, **GPIO48**, SUBSPICLK_N_DIFF                                                        |



GPIO47 was seen 3.3V on some Modules. 


