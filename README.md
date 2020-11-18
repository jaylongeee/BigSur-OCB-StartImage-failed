# BigSur-OCB-StartImage-failed
Get this message when trying to install Open Core BigSur 11.0.1

I have done my best to read up solutions but not have got anywhere like BlessOverride, played around with various BIOS settings
Intel Core i9 9900K, S 1151, Coffee Lake Refresh, 8 Core, 16 Thread, 3.6GHz
Gigabyte Z390, Intel Z390
8GB AMD Radeon RX 580

Here is the full log of install:

00:000 00:000 AAPL: #[EB|LOG:INIT] 2020-11-18T12:30:54
00:073 00:073 AAPL: #[EB|VERSION] <"bootbase.efi 495.40.10~123 (Official), built 2020-10-30T00:10:36-0700">
00:147 00:073 AAPL: #[EB|BUILD] <"BUILD-INFO[310]:{"DisplayName":"bootbase.efi","DisplayVersion":"495.40.10~123","RecordUuid":"E287ED06-5B89-4BD5-82FD-8CF9CD5A1AA7","BuildTime":"2020-10-30T00:10:36-0700","ProjectName":"efiboot","ProductName":"bootbase.efi","SourceVersion":"495.40.10","BuildVersion":"123","BuildConfiguration":"Release","BuildType":"Official"}">
00:221 00:073 AAPL: #[EB|CFG:DEV] r2 0x0 0x0
00:295 00:074 AAPL: #[EB|H:IS] 0
00:368 00:073 AAPL: #[EB|WL:MODE] 0
00:442 00:073 AAPL: #[EB|CFG:ARG] boot-save-log 0x0000000000000002 (0x0000000000000002 < 0xFFFFFFFFFFFFFFFF) default
00:516 00:073 AAPL: #[EB|CFG:ARG] wake-save-log 0x0000000000000002 (0x0000000000000002 < 0x0000000000000002) default
00:589 00:073 AAPL: #[EB|CFG:ARG] console       0x0000000000000001 (0x0000000000000001 < 0x0000000000000001) default
00:663 00:073 AAPL: #[EB|CFG:ARG] serial        0x0000000000000000 (0x0000000000000000 < 0x0000000000000000) default
00:737 00:073 AAPL: #[EB|CFG:ARG] embed-log-dt  0x0000000000000000 (0x0000000000000000 < 0x0000000000000000) default
00:810 00:073 AAPL: #[EB|CFG:ARG] timestamps    0x0000000000000000 (0x0000000000000000 < 0xFFFFFFFFFFFFFFFF) default
00:884 00:073 AAPL: #[EB|CFG:ARG] log-level     0x0000000000000001 (0x0000000000000001 & 0x0000000000000021) default
00:958 00:073 AAPL: #[EB|CFG:ARG] breakpoint    0x0000000000000000 (0x0000000000000000 & 0x0000000000000000) default
01:031 00:073 AAPL: #[EB|CFG:ARG] kc-read-size  0x0000000000100000 (0x0000000000100000 < 0xFFFFFFFFFFFFFFFF) default
01:170 00:138 AAPL: #[EB|H:IS] 0
01:243 00:073 AAPL: #[EB|WL] 0 0 0x01 0x01   0 0x00
01:316 00:073 AAPL: #[EB|BRD:NV] Mac-7BA5B2D9E42DDD94
01:389 00:073 AAPL: #[EB|WL] 0 0 0x01 0x01   2 0x00
01:463 00:073 AAPL: #[EB.BST.IDT|+]
01:537 00:074 AAPL: #[EB.BST.IDT|-]
01:610 00:073 AAPL: #[EB|WL] 0 0 0x01 0x01   3 0x00
01:683 00:073 AAPL: #[EB|WL] 0 0 0x01 0x01   4 0x00
01:756 00:073 AAPL: #[EB|BRD:NV] Mac-7BA5B2D9E42DDD94
01:829 00:072 AAPL: #[EB|WL] 0 0 0x01 0x01   5 0x00
01:902 00:072 AAPL: #[EB.H.CHK|BM] 0x0000000000000000
01:975 00:073 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.GV boot-signature 7C436110-AB2A-4BBB-A880-FE41995C9F82
02:049 00:073 AAPL: #[EB|WL] 0 0 0x01 0x01  23 0x0E
02:122 00:073 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.GV boot-image-key 7C436110-AB2A-4BBB-A880-FE41995C9F82
02:196 00:073 AAPL: #[EB|WL] 0 0 0x01 0x01  24 0x0E
02:269 00:073 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.GV boot-image 7C436110-AB2A-4BBB-A880-FE41995C9F82
02:343 00:073 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.SV- boot-signature 7C436110-AB2A-4BBB-A880-FE41995C9F82
02:417 00:073 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.SV- boot-image-key 7C436110-AB2A-4BBB-A880-FE41995C9F82
02:491 00:073 AAPL: #[EB.H.LV|!] Err(0xE) <- RT.SV- boot-image 7C436110-AB2A-4BBB-A880-FE41995C9F82
02:564 00:073 AAPL: #[EB|H:NOT]
02:638 00:073 AAPL: #[EB|SB:P] 0x1
02:711 00:073 AAPL: #[EB.B.MN|BM:+SB]
02:785 00:073 AAPL: #[EB|LIMG:DP] Acpi(PNP0A03,0)/Pci(14|0)/Usb(7, 0)/HD(Part2,SigD2FC2839-74F3-4824-B85C-326C55C64CF7)
02:858 00:073 AAPL: #[EB|LIMG:FP] \System\Library\CoreServices\boot.efi
02:932 00:073 AAPL: #[EB|LIMG:OPT] 
03:107 00:175 AAPL: #[EB|RPS] 0 0 0
03:182 00:074 AAPL: #[EB.OPT.LXF|F] <"\\System\\Library\\CoreServices\\com.apple.Boot.plist">
03:255 00:073 AAPL: #[EB.LD.LF|IN] 0 1 <"\\System\\Library\\CoreServices\\com.apple.Boot.plist"> <"0">
03:328 00:072 AAPL: #[EB.LD.OFS|OPEN!] Err(0xE) <"\\System\\Library\\CoreServices\\com.apple.Boot.plist">
03:401 00:072 AAPL: #[EB.OPT.LXF|LF!] Err(0xE)
03:474 00:072 AAPL: #[EB.OPT.LXF|F] <"Library\\Preferences\\SystemConfiguration\\com.apple.Boot.plist">
03:547 00:073 AAPL: #[EB.LD.LF|IN] 0 1 <"Library\\Preferences\\SystemConfiguration\\com.apple.Boot.plist"> <"0">
03:629 00:082 AAPL: #[EB|KF] <"root-dmg=file:///BaseSystem/BaseSystem.dmg">
03:703 00:073 AAPL: #[EB|MBA:CL] <"">
03:776 00:073 AAPL: #[EB|MBA:NV] <"-v keepsyms=1 debug=0x100 npci=0x2000 alcid=1 slide=0  ">
03:849 00:073 AAPL: #[EB|MBA:KF] <"root-dmg=file:///BaseSystem/BaseSystem.dmg">
03:922 00:073 AAPL: #[EB|MBA:OUT] <"-v keepsyms=1 debug=0x100 npci=0x2000 alcid=1 slide=0  root-dmg=file:///BaseSystem/BaseSystem.dmg chunklist-security-epoch=0 -chunklist-no-rev2-dev">
03:996 00:073 AAPL: #[EB|LOG:VERBOSE] 2020-11-18T12:30:58
04:070 00:073 AAPL: #[EB.CSR.S|VAR] 0x000003E7
04:143 00:073 AAPL: #[EB|OPT:BM] 0x200082
04:217 00:073 AAPL: #[EB.OPT.LXF|F] <"\\System\\Library\\CoreServices\\PlatformSupport.plist">
04:291 00:073 AAPL: #[EB.LD.LF|IN] 0 1 <"\\System\\Library\\CoreServices\\PlatformSupport.plist"> <"0">
04:366 00:075 AAPL: #[EB|B:VAw]
04:440 00:073 AAPL: #[EB|P:CPR] N
04:513 00:073 AAPL: #[EB|P:MPI] N
04:587 00:073 AAPL: #[EB|P:BPI] N
04:661 00:073 AAPL: #[EB.MM.AKMR|!] Err(0xE) <- EB.M.BAP 122209
04:734 00:073 AAPL: #[EB.B.MN|!] Err(0xE) <- EB.MM.AKMR
04:808 00:073 AAPL: #[EB|WL] 0 0 0x01 0x03  24 0x0E
04:882 00:073 AAPL: #[EB|STOP]
05:063 00:181 AAPL: #[EB|WL] 0 0 0x01 0x03  24 0x0E
05:136 00:072 AAPL: #[EB|LOG:EXIT] 2020-11-18T12:30:59
15:210 10:074 OC: Boot failed - Aborted
15:283 00:072 OCB: StartImage failed - Aborted
