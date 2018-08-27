# LoRa-GateWay-Cfg
The configuration file required by the packet forwarder in LoRa GateWay at https://github.com/Lora-net/packet_forwarder

How to use(here is SX1301+raspberry pi):

$cd home

$sudo git clone https://github.com/Lora-net/lora_gateway.git

$sudo git clone https://github.com/Lora-net/packet_forwarder.git  

$cd lora_gateway

$sudo make

$cd ..


$cd packet_forwarder
$sudo make

use ssh/putty copy those JSON files to /home/packet_forwarder/lora_pkt_fwd/,then change some configuration by

$sudo nano /home/packet_forwarder/lora_pkt_fwd/global_conf_eu434.json

after change frequency localhost... then

$ln -sf global_conf_eu434.json global_conf.json
