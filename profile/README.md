<p align="center">
  <img src="https://raw.githubusercontent.com/Cloudopsshell/.github/main/profile/assets/deaconguard-shield.svg" width="64" height="64" alt="">
</p>

<h1 align="center">DeaconGuard</h1>

<p align="center">
  A Linux security scanner with a central server and enrollment-token agents. It checks packages against the official Ubuntu, Debian, RHEL and Amazon Linux advisories and covers file integrity, security configuration and malware (ClamAV, plus optional YARA-X rules).
</p>

<p align="center">
  <a href="https://github.com/Cloudopsshell/deaconguard/releases/latest"><img src="https://img.shields.io/github/v/release/Cloudopsshell/deaconguard?style=flat-square&label=release&color=1a7f37" alt="Latest release"></a>
  <a href="https://github.com/Cloudopsshell/deaconguard/blob/main/LICENSE"><img src="https://img.shields.io/github/license/Cloudopsshell/deaconguard?style=flat-square&label=license&color=0969da" alt="License"></a>
  <img src="https://img.shields.io/badge/go-00758f?style=flat-square&logo=go&logoColor=white" alt="Go">
  <img src="https://img.shields.io/badge/releases-cosign--signed-6639ba?style=flat-square" alt="Releases signed with cosign">
</p>

```sh
# Server
curl -fsSL https://get.deaconguard.io | sudo sh -

# Agent, with the one-time token from the server's Agents page
curl -fsSL https://get.deaconguard.io | DEACONGUARD_TOKEN=deaconguard1.... sudo -E sh -
```

<table>
  <tr>
    <td width="50%"><b>Vulnerable packages</b><br>Matched against vendor advisories for Ubuntu, Debian, RHEL and Amazon Linux.</td>
    <td width="50%"><b>File integrity</b><br>Spots changes to the files that matter on each host.</td>
  </tr>
  <tr>
    <td width="50%"><b>Malware scanning</b><br>ClamAV by default, YARA-X rules for the advanced scan.</td>
    <td width="50%"><b>Security configuration</b><br>Checks how each machine is set up, not just what is installed.</td>
  </tr>
</table>

<p align="center">
  <a href="https://deaconguard.io">Website</a> · <a href="https://docs.deaconguard.io">Docs</a> · <a href="https://github.com/Cloudopsshell/deaconguard/releases">Releases</a>
</p>

---

**Also from CloudOpsShell:** [xferctl](https://github.com/Cloudopsshell/xferctl) v1.0.1, a CLI for copying files between S3 buckets, including across AWS accounts.
