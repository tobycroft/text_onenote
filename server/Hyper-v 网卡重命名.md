$VMNetAdap = Get-VMNetworkAdapter -VMName Router

Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[0] -NewName "Eth0"



Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[1] -NewName "Eth1"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[2] -NewName "Eth2"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[3] -NewName "Eth3"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[4] -NewName "Eth4"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[5] -NewName "Eth5"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[6] -NewName "Eth6"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[7] -NewName "Eth7"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[8] -NewName "Eth8"

Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[9] -NewName "Eth9"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[10] -NewName "Eth10"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[11] -NewName "Eth11"
Rename-VMNetworkAdapter -VMNetworkAdapter $VMNetAdap[12] -NewName "Eth12"




Set-VMNetworkAdapterVlan -VMName Router -VMNetworkAdapterName "Eth0" -Trunk -AllowedVlanIdList "1-4094" -NativeVlanId 0
Set-VMNetworkAdapterVlan -VMName Router -VMNetworkAdapterName "Eth1" -Trunk -AllowedVlanIdList "1-4094" -NativeVlanId 0
Set-VMNetworkAdapterVlan -VMName Router -VMNetworkAdapterName "Eth2" -Trunk -AllowedVlanIdList "1-4094" -NativeVlanId 0

Set-VMNetworkAdapterVlan -VMName Router -VMNetworkAdapterName "Eth0" -Untagged
