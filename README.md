# CryptoDonkeyMinersTuningTool (Autolykos2 / Ethash / Kawpow / Octopus)

CryptoDonkeyMinersTuningTool will help you find the best overclock settings for your Nvidia GPU. It will go through the specified (core clock, memory clock, power limit) and add the results to an easy-to-sort list, to help you find the best overclocking or underclock for your card.

Currently only Ergo (ERG), Conflux (CFX), Ethereum (ETH) and Ravencoin (RVN) with T-Rex miner are supported.

V1.0.0 ERG video demo: https://youtu.be/htG0PyrHgtQ

V1.0.2 RVN video demo: https://youtu.be/9S977sqvpCQ

My YouTube Channel: https://www.youtube.com/channel/UCXpeiHGQziOKLA1P1sGUFkA

(You really need to check my YouTube out if you have a newer version LHR GPU, like the RTX 3070 LHR and RTX 3060 LHR V2, and want to mine ERGO)

RTX 3060 LHR V2 mining ERGO 103 MH/s at 78 watts: https://youtu.be/yDbIE3XNs5Q

RTX 3070 LHR mining ERGO 135 MH/s at 89 watts: https://youtu.be/A0uvAqr1d8U

## Options
* **Coins**</br>
```
Select the coin you want to tune your card towards
```

* **Core Clock**</br>
```
* FROM
Where the core tuning should start from
* TO
Where the core tuning should end 
* INCREMENT
For each complete running iteration, increment will be added to FROM and stop the tuning when it reaches TO
```

* **Memory Clock**</br>
```
* FROM
Where the memory tuning should start from
* TO
Where the memory tuning should end 
* INCREMENT
For each complete running iteration, increment will be added to FROM and move to the next core clock when TO has been reached
```

* **Power Limit**</br>
```
* FROM
Where the power limit tuning should start from
* TO
Where the power limit tuning should end 
* INCREMENT
For each complete running iteration, increment will be added to FROM and move to the next memory clock when TO has been reached
```

* **Core Clock Locked**</br>
```
* When checked Power Limit will be disabled, as T-Rex Miner will set the Core Clock to a fixed rate, that will determin the power usage
* WHen uncheck Power Limit will be enabled and it is up to you to define the range
```

* **Hashrate**</br>
```
* Minimum
The minimum acceptable hashrate before retries are triggered
* Retries
Amount of times (T-Rex summary displayed) a specific combination of clocks and power limit should run, before moving on.
Use this if you have problems with your current OC falling off a cliff after running completely stable for some time
```

* **GPU**</br>
```
* The GPU number you want to test (if you only have 1 GPU, it should be set to 0)
```

* **Wallet**</br>
```
* Your wallet for the specific selected cryptocurrency. Default is DEV Wallet.
```

* **T-Rex Path**</br>
```
* The path to the folder where your t-rex.exe is. Example: Your t-rex.exe full path is c:\t-rex\t-rex.exe, so path should be set to c:\t-rex
```

DEV FEE:
Every 1 out of 10 times running (with the exception of retries, as it would disrupt stability testing), it will switch to DEV Wallet.


Please report bugs and post feature requests here, as I am actively developing the tool :)
