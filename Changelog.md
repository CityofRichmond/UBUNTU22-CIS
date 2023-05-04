# v0.9 Ubuntu22cis v1.0.0

## April 2023 Updates
- Yamllint Check
- Ansible-lint Check
- Fqcn[canonical] module name 
- PR's Addressed
  - [#21](https://github.com/ansible-lockdown/UBUNTU22-CIS/pull/21) - #Thanks @IdrisDose
- Bugs Fixed
  - [#13](https://github.com/ansible-lockdown/UBUNTU22-CIS/issues/13) - Thanks @vdmkenny
  - [#14](https://github.com/ansible-lockdown/UBUNTU22-CIS/issues/14) - Thanks @bgro
  - [#15](https://github.com/ansible-lockdown/UBUNTU22-CIS/issues/15) - Thanks @bgro
  - [#16](https://github.com/ansible-lockdown/UBUNTU22-CIS/issues/16) - Thanks @bgro
  - [#17](https://github.com/ansible-lockdown/UBUNTU22-CIS/issues/17) - Thanks @bgro
  - [#18](https://github.com/ansible-lockdown/UBUNTU22-CIS/issues/18) - Thanks @bgro
  - [#19](https://github.com/ansible-lockdown/UBUNTU22-CIS/issues/19) - Thanks @bgro
  - [#20](https://github.com/ansible-lockdown/UBUNTU22-CIS/issues/20) - Thanks @bgro

## Initial ubuntu22cis release

- Ansible 2.10.1 minimum
- fqcns added
- audit alignment to use corresponding benchamrk version
- many lint improvements
- All required changes for CIS 1.0.0 (very different from original base of ubuntu2004)

### New options

- default firewall now ufw

- If firewall = UFW to use system sysctl settings: default
  - _ubtu22cis_ufw_use_sysctl: true_

- Abilty to set alternate sysctl file for network settings: default
  - _ubtu22cis_sysctl_network_conf: /etc/sysctl.conf_

- Abilty to set syslog service: choose between rsyslog or journald: default
  - _ubtu22cis_syslog_service: rsyslog_
