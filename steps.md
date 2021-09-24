1.install esp-idf to env var by running the install.sh and . ./export.sh
2.micropython folder:
 idf.py set-target esp32    --> this will erase all menuconfig
 idf.py menuconfig --> enable 80Mhz, SPIRAM
 git submodule update --init -recursive
 make BOARD=GENERIC_CAM deploy    --> this will build the generic cam profile and flash the chip.