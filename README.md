<div align="center">

<img src="https://3eed.page.gd/dragon.svg" width="92" height="92" alt="dragon" />

# dragon

<p>
  <a href="https://3eed.page.gd"><img src="https://img.shields.io/badge/Site-3eed.page.gd-0D1117?style=flat-square&logo=googlechrome&logoColor=white" alt="Site" /></a>
  <a href="https://bsky.app/profile/riotemployee.bsky.social"><img src="https://img.shields.io/badge/Bluesky-@riotemployee-0285FF?style=flat-square&logo=bluesky&logoColor=white" alt="Bluesky" /></a>
  <a href="https://discord.com/users/1330197919797743617"><img src="https://img.shields.io/badge/Discord-dragon-5865F2?style=flat-square&logo=discord&logoColor=white" alt="Discord" /></a>
</p>

```
UEFI DXE -> VMX ROOT -> SECOND-LEVEL ADDRESS TRANSLATION (EPT) -> #VE
```

<blockquote>
From under the hypervisor, the game is memory and nothing else.
</blockquote>

</div>

---

### Architecture & Work

<table>
  <tr>
    <td width="30%"><b>2018</b><br><i>UEFI / Bootkits</i></td>
    <td>
      Resident in DXE runtime before operating system initialization.<br>
      Zero on-disk image, zero loader callbacks, zero object enumeration in user mode.
    </td>
  </tr>
  <tr>
    <td><b>2021</b><br><i>Hypervisors</i></td>
    <td>
      Hypervisor engineering for anti-cheat bypasses.<br>
      VMX root mode, independent VMCS per guest, second-level translation via EPT, and #VE handlers redirecting execution back to custom VMMs.
    </td>
  </tr>
  <tr>
    <td><b>2021</b><br><i>Commercial Services</i></td>
    <td>
      Core engine architecture for <b>Majesty</b>, <b>88Software</b>, and <b>Vanuri</b>.<br>
      Unified low-level kernel codebase supporting multiple isolated deployments simultaneously.
    </td>
  </tr>
  <tr>
    <td><b>ZeroTrace</b><br><i>Public Release</i></td>
    <td>
      <b>DXE Spoofer:</b> Overwrites SMBIOS UUID, disk and motherboard serials, and machine GUID prior to NT kernel load.<br>
      <b>EPT Hypervisor:</b> Passive memory inspector inside VMX root. Reads memory through physical paging without writing to target address spaces.
    </td>
  </tr>
</table>

---

### Stack & Toolchain

<p>
  <img src="https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white" alt="C" />
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/Assembly_x86--64-333333?style=flat-square" alt="Assembly" />
  <img src="https://img.shields.io/badge/UEFI_EDK_II-1B1F23?style=flat-square" alt="UEFI" />
  <img src="https://img.shields.io/badge/Windows_Kernel-0078D4?style=flat-square&logo=windows&logoColor=white" alt="Windows Kernel" />
  <img src="https://img.shields.io/badge/VMX_Root_EPT-111111?style=flat-square" alt="VMX" />
  <img src="https://img.shields.io/badge/IDA_Pro-0A2F44?style=flat-square" alt="IDA Pro" />
  <img src="https://img.shields.io/badge/x64dbg-2A2A2A?style=flat-square" alt="x64dbg" />
  <img src="https://img.shields.io/badge/WinDbg-004E8C?style=flat-square" alt="WinDbg" />
</p>

---

### Publications

- [What I have built so far](https://3eed.page.gd/article.php?slug=2026-10-10-what-i-have-built)
- [2023, reversing vgk.sys internals and the audiodg manual mapper](https://3eed.page.gd/article.php?slug=2026-10-12-reversing-vanguard-audiodg-injection)

<div align="center">
<sub>&copy; 2026 dragon &bull; <a href="https://3eed.page.gd">3eed.page.gd</a></sub>
</div>
