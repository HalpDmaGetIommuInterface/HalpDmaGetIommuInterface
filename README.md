<div align="center">

<img src="./dragon.svg" width="110" height="110" alt="dragon" />

# dragon

<a href="https://3eed.page.gd"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=16&pause=1000&color=FFFFFF&center=true&vCenter=true&width=620&lines=i+write+rootkits%2C+bootkits+and+hypervisors.;malware+analysis+%2F+vulnerability+research;offensive+security+%2F+exploit+development;ring+0+and+below+%E2%80%A2+from+under+the+hypervisor." alt="dragon console" /></a>

<br/>

<a href="https://3eed.page.gd">
  <img src="https://img.shields.io/badge/3eed.page.gd-000000?style=for-the-badge&logo=target&logoColor=white" alt="3eed.page.gd" />
</a>
&nbsp;
<a href="https://bsky.app/profile/riotemployee.bsky.social">
  <img src="https://img.shields.io/badge/Bluesky-0285FF?style=for-the-badge&logo=bluesky&logoColor=white" alt="Bluesky" />
</a>
&nbsp;
<a href="https://discord.com/users/1330197919797743617">
  <img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" />
</a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:000000,100:1a1a1a&height=4&width=100%" alt="divider" />

</div>

### Identity & Parameters

```ini
[identity]
handle    = dragon
since     = 2018
age       = 24
status    = working
access    = ring 0 and below
targets   = windows, linux
location  = unknown

[focus]
domains   = malware analysis / vulnerability research / offensive security / exploit development
specialty = rootkits, bootkits, hypervisors

[languages]
core      = c, c++, c#, asm, python, bash
site      = php, js, css
```

---

### Low-Level Architecture & Execution

<table>
  <thead>
    <tr>
      <th align="left">Vector</th>
      <th align="left">Technical Scope</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>Bootkits & UEFI</b><br><code>2018 &mdash; Present</code></td>
      <td>
        Hooked into DXE driver dispatch before OS initialization.<br>
        Zero file on disk, zero PE hash, zero ObRegisterCallbacks handle tracking.
      </td>
    </tr>
    <tr>
      <td><b>Hypervisor Virtualization</b><br><code>2021 &mdash; Present</code></td>
      <td>
        VMX root operation with dedicated VMCS execution controls.<br>
        Second-level address translation (EPT) to observe guest address spaces passively without in-process injection or hooks.
      </td>
    </tr>
    <tr>
      <td><b>Offensive Engines</b><br><code>Majesty / 88Software / Vanuri</code></td>
      <td>
        Architected shared low-level core for three independent commercial services concurrently.<br>
        Isolated deployment surface over unified ring-0 driver mechanics.
      </td>
    </tr>
    <tr>
      <td><b>ZeroTrace</b><br><code>Public Release</code></td>
      <td>
        <b>DXE Spoofer:</b> Intercepts and rewrites disk serial, board serial, SMBIOS UUID, and machine GUID before the NT kernel loads.<br>
        <b>EPT Hypervisor:</b> Passive memory inspector inside VMX root. Reads memory through physical paging without writing to target address spaces.
      </td>
    </tr>
  </tbody>
</table>

---

### Stack & Instrumentation

<div align="center">

```
[ REVERSING ]   IDA Pro  •  x64dbg  •  WinDbg
[ RUNTIME ]     UEFI EDK II  •  Windows Kernel  •  VMX Root
[ LANGUAGES ]   C  •  C++  •  C#  •  x86_64 ASM  •  Python  •  Bash
```

</div>

---

### Publications

- [What I have built so far](https://3eed.page.gd/article.php?slug=2026-10-10-what-i-have-built)
- [2023, reversing vgk.sys internals and the audiodg manual mapper](https://3eed.page.gd/article.php?slug=2026-10-12-reversing-vanguard-audiodg-injection)

<div align="center">
<sub>&copy; 2026 dragon &bull; <a href="https://3eed.page.gd">3eed.page.gd</a></sub>
</div>
