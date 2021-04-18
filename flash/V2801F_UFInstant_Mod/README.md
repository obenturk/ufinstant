###replaced files

/bin/diag
/bin/europacli
/bin/busybox

chown 1013
chmod 775


###added files
/lib/modules/europa_drv.ko

chown 1013
chmod 664

###changed files

####rc2
'''
mkdir /var/hw

mount -t jffs2 -o ro /dev/mtdblock8 /var/hw
if [[ -f /var/hw/europa.data ]]; then
	if ! cmp /var/config/europa.data /var/hw/europa.data -s; then
                echo "Copy /var/hw/europa.data /var/config/europa.data"
                cp -f /var/hw/europa.data /var/config/europa.data
	fi
elif [[ ! -f  /var/config/europa.data ]]; then
    echo "Warning: File /var/hw/europa.data nor /var/config/europa.data doesn't exist!!!. Generating."
    /bin/europacli open default
fi
'''
####rc32
'''
insmod /lib/modules/europa_drv.ko PON_MODE=1 I2C_PORT=1 INTR_PIN=0 TXDIS_PIN=13 TXPWR_PIN=15