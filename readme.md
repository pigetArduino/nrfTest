# Wiring
**nrf modules use 3.3V not 5V**

![nrf_pinout](https://github.com/pigetArduino/milightONOFF/raw/master/doc/nrf_pinout.png)

![touchsensor](https://github.com/pigetArduino/milightONOFF/raw/master/doc/touchsensor.png)

```
NRF
D9	: orange
D10	: yellow
D11	: blue
D12	: purple
D13	: green
3.3V: red

SWITCHS
D4	OFF SIG
D5	ON SIG
5V: VCC
```

## Check radio module
You should see your radio module parameters, if all parameters are set to **0x00**, the module is not correctly wired       
**Example** 
```
STATUS		 = 0x0e RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=7 TX_FULL=0
RX_ADDR_P0-1	 = 0xe7e7e7e7e7 0xc2c2c2c2c2
RX_ADDR_P2-5	 = 0xc3 0xc4 0xc5 0xc6
TX_ADDR		 = 0xe7e7e7e7e7
RX_PW_P0-6	 = 0x00 0x00 0x00 0x00 0x00 0x00
EN_AA		 = 0x3f
EN_RXADDR	 = 0x03
RF_CH		 = 0x4c
RF_SETUP	 = 0x07
NRF_CONFIG		 = 0x0e
DYNPD/FEATURE	 = 0x00 0x00
Data Rate	 = 1MBPS
Model		 = nRF24L01+
CRC Length	 = 16 bits
PA Power	 = PA_MAX
```