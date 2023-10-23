Get-VMNetworkAdapterVlan -VMName Route


Set-VMNetworkAdapterVlan -VMName Route -VMNetworkAdapterName "Eth3" -Trunk -AllowedVlanIdList "1-4094" -NativeVlanId "0"






