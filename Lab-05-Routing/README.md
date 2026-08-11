# Lab 04 – Virtual Local Area Networks (VLANs)

## Objective

Create VLANs on a Cisco switch, assign switch ports to VLANs, and verify communication between devices.

## Devices Used

| Device | Quantity |
|---------|---------:|
| PC | 3 |
| Cisco 2960 Switch | 1 |

## VLAN Configuration

| VLAN ID | Name | Ports |
|---------|------|-------|
| 10 | HR | Fa0/1, Fa0/2 |
| 20 | Finance | Fa0/3 |

## IP Addressing

| Device | IP Address | VLAN |
|---------|------------|------|
| PC0 | 192.168.10.10 | 10 |
| PC1 | 192.168.10.20 | 10 |
| PC2 | 192.168.20.10 | 20 |

## Verification

- PC0 successfully pinged PC1.
- PC0 could not ping PC2 because they belong to different VLANs.

## Troubleshooting

Moved PC1 to VLAN 20, observed communication failure with PC0, then restored PC1 to VLAN 10 and verified successful communication.

## Skills Learned

- Creating VLANs
- Naming VLANs
- Assigning switch ports to VLANs
- Verifying VLAN configuration
- Troubleshooting VLAN issues

## Common Mistakes

- Forgetting to assign ports to the correct VLAN.
- Assuming devices on the same switch can always communicate.
- Forgetting to save the switch configuration.

## Cybersecurity Connection

VLANs improve network segmentation and reduce unnecessary communication between departments. SOC analysts use VLAN knowledge to investigate unauthorized access, identify network segmentation issues, and understand potential VLAN hopping attacks.
