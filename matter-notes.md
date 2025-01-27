# tapo L535E smart wifi light bulb
```
demo discover commissionable --timeout 3
MatterDeviceInfo {
    service: "C978030681EE29B7",
    device: "B01921FBDB87",
    ips: [
        192.168.5.201,
        fdf4::96a,
        fdf4::b219:21ff:fefb:db87,
        fe80::b219:21ff:fefb:db87,
    ],
    name: Some(
        "Smart Multicolor Bulb",
    ),
    discriminator: Some(
        "1871",
    ),
    commissioning_mode: Some(
        WithPasscode,
    ),
    pairing_hint: Some(
        "36",
    ),
}
```

`demo commission --local-address [fdf4::80a:4b0a:6ddc:8216]:5555 [fdf4::b219:21ff:fefb:db87]:5540 100 300 65659274`

`demo command invoke-command-on --local-address [fdf4::80a:4b0a:6ddc:8216]:5555   --device-address [fdf4::b219:21ff:fefb:db87]:5540`

`demo command invoke-command-off --local-address [fdf4::80a:4b0a:6ddc:8216]:5555   --device-address [fdf4::b219:21ff:fefb:db87]:5540`

```
demo command list-supported-clusters2 --local-address [fdf4::80a:4b0a:6ddc:8216]:5555   --device-address [fdf4::b219:21ff:fefb:db87]:5540 0
Descriptor
AccessControl
Basic Information
OTA Software Update Requestor
General Commissioning
Network Commissioning
General Diagnostics
Administrator Commissioning
Operational Credentials
GroupKeyManagement
```

```
demo command list-supported-clusters2 --local-address [fdf4::80a:4b0a:6ddc:8216]:5555   --device-address [fdf4::b219:21ff:fefb:db87]:5540 1
Identify
Groups
unknown cluster - id 0x5
On/Off
Level Control
Descriptor
Color Control
```
