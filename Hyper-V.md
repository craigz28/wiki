## Broadcom NICs

If your Hyper-V host uses Broadcom cards and you are experiencing slow VM network speeds, try disabling Virtual Machine Queues in the Advanced tab of your NIC used to transmit and receive VM network traffic. Speeds should increase to normal once disabled.

## Capturing VM traffic

If you are looking to capture network traffic from your VMs, check out the Advanced Networking feature in the settings for your VM. Under Mirroring you select Source or Destination depending on whether that particular VM is capturing the traffic or sending to another VM that is capturing the traffic.
