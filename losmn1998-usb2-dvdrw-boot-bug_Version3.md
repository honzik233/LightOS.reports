# Boot failure: 'error 666 unknown' with USB 2.0 and DVD-RW media on LOSMN-1998 (LightOS 2.0 LSP4)

**Summary:**  
On machine LOSMN-1998, attempting to boot the LightOS 2.0 LSP4 installer (build 0001) results in an "error 666 unknown" when using USB 2.0 drives or DVD-RW media. Booting from BD/DVD±R/CD and USB 3.0 works without issue.

**Details:**
- **Machine:** LOSMN-1998
- **LightOS Version:** 2.0 LSP4 (installer build 0001; ancient build)
- **Error:** 666 unknown during boot
- **Boot Media:**
  - USB 2.0: Fails with error 666 unknown
  - DVD-RW: Fails to boot
  - USB 3.0: Boots successfully
  - BD/DVD±R/CD: Boots successfully

**Steps to Reproduce:**
1. Prepare LightOS 2.0 LSP4 installer (build 0001) on a USB 2.0 flash drive or DVD-RW disc.
2. Attempt to boot the installer on LOSMN-1998.
3. Observe the error 666 unknown when booting from USB 2.0, or failure to boot from DVD-RW.
4. Note that USB 3.0 and BD/DVD±R/CD media boot as expected.

**Expected Behavior:**  
The installer should boot from all standard supported media, including USB 2.0 and DVD-RW.

**Actual Behavior:**  
Boots only from USB 3.0 and BD/DVD±R/CD. USB 2.0 and DVD-RW fail as described above.

**Additional Info:**
- BIOS/UEFI settings were checked and adjusted, but did not resolve the issue.
- Multiple USB sticks and ports have been tested.
- The issue persists only with USB 2.0 and DVD-RW; newer media types and other optical discs work properly.
- No screenshots are available at this time.

**Impact:**  
This affects users attempting to install LightOS 2.0 LSP4 on hardware limited to USB 2.0 or DVD-RW boot options, reducing installation flexibility and compatibility.

**Suggested Actions:**
- Investigate bootloader or media compatibility issues for USB 2.0 and DVD-RW on the affected hardware.
- Consider updating the installer, bootloader, or documentation to address or note these limitations.

_Reported by honzik233 to LightOS.Inc_