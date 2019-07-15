# openwrt_MT7688_loragw and pkt_forwarder
Mediatek MT7688/MT7628 openwrt 15.05 Semtech LORAGW 5.0 and packet_forwarder 4.0.0.1

How to

a.) flash firmware from https://docs.labs.mediatek.com/resource/linkit-smart-7688/en/downloads

b.) config MT7688 as station with you Wifi and set root password

c:) Winscp > scp connection with your device

c:) transfer the files to /tmp/

d:) putty ssh with your device

e:) install ipk packages

    opkg install /tmp/libmpsse_1.3.1-1_ramips_24kec.ipk
    
    opkg install /tmp/lora-gateway_5.0.1-1_ramips_24kec.ipk
    
    opkg install /tmp/packet_forwarder_4.0.1-1_ramips_24kec.ipk
    
f:) 
The configuration files for packet_forwarder are located here 
    (vi is just installed with the firmware)

    /bin/usr/packet_forwarder
    
g:) Start LORA Gateway with this command

    /usr/bin/packet_forwarder/ ./lora_pkt_fwd

Enjoy it! :-)


    

    

    

    
