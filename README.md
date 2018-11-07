# Install MEGACLI (Ubuntu)
  Ramin Hakimi
## Install:
	dpkg -i megacli_8.07.14-1_amd64.deb
	
## Command Line:

	== Installation Check ==
  	megacli -LDInfo -Lall -aALL

	== Controller information ==
  	megacli -AdpAllInfo -aALL

	== Enclosure information ==
  	megacli -EncInfo -aALL

	== Virtual drive information ==
  	megacli -LDInfo -Lall -aALL

	== Physical drive information ==
  	megacli -PDList -aALL
  	megacli -PDInfo -PhysDrv [E:S] -aALL

	== Battery backup information ==
  	megacli -AdpBbuCmd -aALL

	== Mark as missing ==
  	megacli -PDMarkMissing -PhysDrv [E:S] -aN

	== Prepare for removal ==
  	megacli -PdPrpRmv -PhysDrv [E:S] -aN

	== Prepare for removal ==
  	megacli -PdReplaceMissing -PhysDrv [E:S] -ArrayN -rowN -aN

	== Show progress ==
  	megacli -PDRbld -ProgDsply -PhysDrv [E:S] -aALL

	== LED Blink ==
  	megacli -PdLocate -start -physdrv[E:S] -a0
  
	== Stop Beeping ==
  	megacli -AdpSetProp AlarmDsbl -aALL 
  
	== Start Beeping again ==
  	megacli -AdpSetProp AlarmEnbl -aALL
