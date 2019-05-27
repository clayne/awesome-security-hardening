# awesome-security-hardening

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A collection of awesome security hardening guides, best practices, tools and other resources.
This is work in progress: please contribute by sending your suggestions. You may do this by creating [issue tickets](https://github.com/decalage2/awesome-security-hardening/issues) or forking, editing and sending pull requests. You may also send suggestions on Twitter to [@decalage2](https://twitter.com/decalage2), or use https://www.decalage.info/contact

------
# Table of Contents

- [Security Hardening Guides and Best Practices](#security-hardening-guides-and-best-practices)
  - [Hardening Guide Collections](#hardening-guide-collections)
  - [GNU/Linux](#gnulinux)
    - [Red Hat Enterprise Linux - RHEL](#red-hat-enterprise-linux---rhel)
    - [SUSE](#suse)
    - [Ubuntu](#ubuntu)
  - [Windows](#windows)
  - [macOS](#macos)
  - [Network Devices](#network-devices)
    - [Switches](#switches)
    - [Routers](#routers)
    - [IPv6](#ipv6)
  - [Virtualization - VMware](#virtualization---vmware)
  - [Containers - Docker](#containers---docker)
  - [Services](#services)
    - [SSH](#ssh)
    - [TLS/SSL](#tlsssl)
    - [Web Servers](#web-servers)
      - [Apache HTTP Server](#apache-http-server)
      - [Apache Tomcat](#apache-tomcat)
      - [Eclipse Jetty](#eclipse-jetty)
      - [Microsoft IIS](#microsoft-iis)
    - [Mail Servers](#mail-servers)
    - [FTP Servers](#ftp-servers)
    - [Database Servers](#database-servers)
    - [Active Directory](#active-directory)
    - [ADFS](#adfs)
    - [Kerberos](#kerberos)
    - [LDAP](#ldap)
    - [DNS](#dns)
    - [NTP](#ntp)
    - [NFS](#nfs)
    - [CUPS](#cups)
  - [Authentication - Passwords](#authentication---passwords)
  - [Hardware - BIOS - UEFI](#hardware---bios---uefi)
  - [Cloud](#cloud)
- [Tools](#tools)
  - [Tools to check security hardening](#tools-to-check-security-hardening)
    - [GNU/Linux](#gnulinux-1)
    - [Network Devices](#network-devices-1)
    - [TLS/SSL](#tlsssl-1)
    - [Docker](#docker)
  - [Tools to apply security hardening](#tools-to-apply-security-hardening)
    - [GNU/Linux](#gnulinux-2)
    - [Windows](#windows-1)
- [Books](#books)
- [Other Awesome Lists](#other-awesome-lists)
  - [Other Awesome Security Lists](#other-awesome-security-lists)

------

# Security Hardening Guides and Best Practices

## Hardening Guide Collections

- [CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks/) (registration required)
- [ANSSI Best Practices](https://www.ssi.gouv.fr/en/best-practices/)
- [NSA Security Configuration Guidance](https://apps.nsa.gov/iaarchive/library/ia-guidance/security-configuration/index.cfm?PAGE=1&itemsQty=ALL)
- [NSA Cybersecurity Resources for Cybersecurity Professionals](https://www.nsa.gov/what-we-do/cybersecurity/) and [NSA Cybersecurity publications](https://nsacyber.github.io/publications.html)
- [US DoD DISA Security Technical Implementation Guides (STIGs) and Security Requirements Guides (SRGs)](https://public.cyber.mil/stigs/)
- [OpenSCAP Security Policies](https://www.open-scap.org/security-policies/)
- [Australian Cyber Security Center Publications](https://www.cyber.gov.au/publications)
- [FIRST Best Practice Guide Library (BPGL)](https://www.first.org/resources/guides/)

## GNU/Linux

- [ANSSI - Configuration recommendations of a GNU/Linux system](https://www.ssi.gouv.fr/en/guide/configuration-recommendations-of-a-gnulinux-system/)
- [CIS Benchmark for Distribution Independent Linux](https://www.cisecurity.org/benchmark/distribution_independent_linux/)
- [How To Secure A Linux Server](https://github.com/imthenachoman/How-To-Secure-A-Linux-Server) - for a single Linux server at home
- [nixCraft - 40 Linux Server Hardening Security Tips (2019 edition)](https://www.cyberciti.biz/tips/linux-security.html)
- [nixCraft - Tips To Protect Linux Servers Physical Console Access](https://www.cyberciti.biz/tips/tips-to-protect-linux-servers-physical-console-access.html)
- [TecMint - 4 Ways to Disable Root Account in Linux](https://www.tecmint.com/disable-root-login-in-linux/)
- [ERNW - IPv6 Hardening  Guide  for  Linux Servers](https://www.ernw.de/download/ERNW_Guide_to_Securely_Configure_Linux_Servers_For_IPv6_v1_0.pdf)

### Red Hat Enterprise Linux - RHEL

- [Red Hat - A Guide to Securing Red Hat Enterprise Linux 7](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html-single/security_guide/index)
- [DISA STIGs - Red Hat Enterprise Linux 7](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=unix-linux) (2019)
- [CIS Benchmark for Red Hat Linux](https://www.cisecurity.org/benchmark/red_hat_linux/)
- [nixCraft - How to set up a firewall using FirewallD on RHEL 8](https://www.cyberciti.biz/faq/configure-set-up-a-firewall-using-firewalld-on-rhel-8/)

### SUSE

- [SUSE Linux Enterprise Server 12 SP4 Security Guide](https://www.suse.com/documentation/sles-12/singlehtml/book_security/book_security.html)
- [SUSE Linux Enterprise Server 12 Security and Hardening Guide](https://www.suse.com/documentation/sles-12/book_hardening/data/book_hardening.html)

### Ubuntu

- [Ubuntu documentation - Security](https://help.ubuntu.com/lts/serverguide/security.html.en)
- [Ubuntu wiki - Security Hardening Features](https://wiki.ubuntu.com/Security/Features)

## Windows

- [Microsoft - Windows security baselines](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-security-baselines)
- [Microsoft - Windows Server Security | Assurance](https://docs.microsoft.com/en-us/windows-server/security/security-and-assurance)
- [Microsoft - Windows 10 Enterprise Security](https://docs.microsoft.com/en-us/windows/security/)
- [ACSC - Hardening Microsoft Windows 10, version 1709, Workstations](https://www.cyber.gov.au/publications/hardening-microsoft-windows-10-build-1709)
- [ACSC - Securing PowerShell in the Enterprise](https://www.cyber.gov.au/publications/securing-powershell-in-the-enterprise)
- [Awesome Windows Domain Hardening](https://github.com/PaulSec/awesome-windows-domain-hardening)
- [Microsoft - How to detect, enable and disable SMBv1, SMBv2, and SMBv3 in Windows and Windows Server](https://support.microsoft.com/en-gb/help/2696547/detect-enable-disable-smbv1-smbv2-smbv3-in-windows-and-windows-server)
- [Microsoft recommended block rules](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/microsoft-recommended-block-rules) - List of applications or files that can be used by an attacker to circumvent application whitelisting policies
- [ERNW - IPv6 Hardening Guide for Windows Servers](https://www.ernw.de/download/ERNW_Guide_to_Configure_Securely_Windows_Servers_For_IPv6_v1_0.pdf)

See also [Active Directory](#active-directory) and [ADFS](#adfs) below.

## macOS

- [ERNW - IPv6 Hardening Guide for OS-X](https://www.ernw.de/download/ERNW_Hardening_IPv6_MacOS-X_v1_0.pdf)

## Network Devices

- [NSA - Harden Network Devices](https://apps.nsa.gov/iaarchive/library/ia-guidance/security-tips/harden-network-devices.cfm) - very short but good summary

### Switches

- [DISA - Layer 2 Switch SRG](http://iasecontent.disa.mil/stigs/zip/U_Layer_2_Switch_V1R3_SRG.zip)

### Routers

- [NSA - A Guide to Border Gateway Protocol (BGP) Best Practices](https://www.nsa.gov/Portals/70/documents/what-we-do/cybersecurity/professional-resources/ctr-guide-to-border-gateway-protocol-best-practices.pdf?v=1)

### IPv6

- ERNW - Developing an Enterprise IPv6 Security Strategy [Part 1](https://www.insinuator.net/2015/12/developing-an-enterprise-ipv6-security-strategy-part-1-baseline-analysis-of-ipv4-network-security/), [Part 2](https://www.insinuator.net/2015/12/developing-an-enterprise-ipv6-security-strategy-part-2-network-isolation-on-the-routing-layer/), [Part 3](https://www.insinuator.net/2015/12/developing-an-enterprise-ipv6-security-strategy-part-3-traffic-filtering-in-ipv6-networks-i/), [Part 4](https://insinuator.net/2015/12/developing-an-enterprise-ipv6-security-strategy-part-4-traffic-filtering-in-ipv6-networks-ii/) - Network Isolation on the Routing Layer, Traffic Filtering in IPv6 Networks
- see also IPv6 links under GNU/Linux, Windows and macOS

## Virtualization - VMware

- [VMware Security Hardening Guides](https://www.vmware.com/security/hardening-guides.html) - covers most VMware products and versions
- [CIS VMware ESXi 6.5 Benchmark](https://www.cisecurity.org/benchmark/vmware/) (2018)
- [DISA STIGs - Virtualisation](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=virtualization) - VMware vSphere 6.0 and 5
- [ENISA - Security aspects of virtualization](https://www.enisa.europa.eu/publications/security-aspects-of-virtualization) - generic, high-level best practices for virtualization and containers (Feb 2017)
- [NIST SP 800-125 - Guide to Security for Full Virtualization Technologies](https://www.nist.gov/publications/guide-security-full-virtualization-technologies) - (2011)
- [ANSSI - Recommandations de sécurité pour les architectures basées sur VMware vSphere ESXi](https://www.ssi.gouv.fr/guide/recommandations-de-securite-pour-les-architectures-basees-sur-vmware-vsphere-esxi/) - for VMware 5.5 (2016), in French

## Containers - Docker

- [How To Harden Your Docker Containers](https://www.secjuice.com/how-to-harden-docker-containers/)
- [CIS Docker Benchmarks](https://www.cisecurity.org/benchmark/docker/) - registration required

## Services

### SSH

- [NIST IR 7966 - Security of Interactive and Automated Access Management Using Secure Shell (SSH)](https://nvlpubs.nist.gov/nistpubs/ir/2015/NIST.IR.7966.pdf)
- [ANSSI - (Open)SSH secure use recommendations](https://www.ssi.gouv.fr/en/guide/openssh-secure-use-recommendations/)
- [Linux Audit - OpenSSH security and hardening](https://linux-audit.com/audit-and-harden-your-ssh-configuration/)
- [Positron Security SSH Hardening Guides](https://www.sshaudit.com/hardening_guides.html) - focused on crypto algorithms

### TLS/SSL

- [NIST SP800-52 Rev 2 (2nd draft) - Guidelines for the Selection, Configuration, and Use of Transport Layer Security (TLS) Implementations](https://csrc.nist.gov/publications/detail/sp/800-52/rev-2/draft) - 2018, recommends TLS 1.3
- [Netherlands NCSC - IT Security Guidelines for Transport Layer Security (TLS)](https://www.ncsc.nl/english/current-topics/factsheets/it-security-guidelines-for-transport-layer-security-tls.html) - 2019
- [ANSSI - Security Recommendations for TLS](https://www.ssi.gouv.fr/en/guide/security-recommendations-for-tls/) - 2017, does not cover TLS 1.3
- [Qualys SSL Labs - SSL and TLS Deployment Best Practices](https://github.com/ssllabs/research/wiki/SSL-and-TLS-Deployment-Best-Practices) - 2017, does not cover TLS 1.3
- [RFC 7540 Appendix A TLS 1.2 Cipher Suite Black List](https://tools.ietf.org/html/rfc7540#appendix-A)

### Web Servers

- [Cipherli.st - Strong Ciphers for Apache, nginx and Lighttpd](https://cipherli.st/)

#### Apache HTTP Server

- [Apache HTTP Server documentation - Security Tips](http://httpd.apache.org/docs/current/misc/security_tips.html)
- [GeekFlare - Apache Web Server Hardening and Security Guide](https://geekflare.com/apache-web-server-hardening-security/)
- [Apache Config - Apache Security Hardening Guide](https://www.apachecon.eu/)

#### Apache Tomcat

- [Apache Tomcat 9 Security Considerations](https://tomcat.apache.org/tomcat-9.0-doc/security-howto.html) / [v8](https://tomcat.apache.org/tomcat-8.0-doc/security-howto.html) / [v7](https://tomcat.apache.org/tomcat-7.0-doc/security-howto.html)
- [OWASP Securing tomcat](https://www.owasp.org/index.php/Securing_tomcat)
- [How to get Tomcat 9 to work with authbind to bind to port 80](https://serverfault.com/questions/889122/how-to-get-tomcat-9-to-work-with-authbind-to-bind-to-port-80)

#### Eclipse Jetty

- [Eclipse Jetty - Configuring Security](https://www.eclipse.org/jetty/documentation/current/configuring-security.html)
- [Jetty hardening](https://virgo47.wordpress.com/2015/02/07/jetty-hardening/) (2015)

#### Microsoft IIS

- [CIS Microsoft IIS Benchmarks](https://learn.cisecurity.org/benchmarks)

### Mail Servers

### FTP Servers

### Database Servers

### Active Directory

- [Microsoft - Best Practices for Securing Active Directory](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/plan/security-best-practices/best-practices-for-securing-active-directory)
- ["Admin Free" Active Directory and Windows, Part 1- Understanding Privileged Groups in AD](https://blogs.technet.microsoft.com/lrobins/2011/06/23/admin-free-active-directory-and-windows-part-1-understanding-privileged-groups-in-ad/)
- ["Admin Free" Active Directory and Windows, Part 2- Protected Accounts and Groups in Active Directory](https://blogs.technet.microsoft.com/lrobins/2011/06/23/admin-free-active-directory-and-windows-part-2-protected-accounts-and-groups-in-active-directory/)

### ADFS

- [adsecurity.org - Securing Microsoft Active Directory Federation Server (ADFS)](https://adsecurity.org/?p=3782)
- [Microsoft - Best practices for securing Active Directory Federation Services](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/deployment/best-practices-securing-ad-fs)

### Kerberos

- [CIS MIT Kerberos 1.10 Benchmark](https://www.cisecurity.org/benchmark/mit_kerberos/) - 2012

### LDAP

- [OpenLDAP Software 2.4 Administrator's Guide - OpenLDAP Security Considerations](http://www.openldap.org/doc/admin24/security.html)
- [Best Practices in LDAP Security](https://www.skills-1st.co.uk/papers/ldap-best-2011/best-practices-in-ldap-security.pdf) (2011)
- [LDAP: Hardening Server Security (so administrators can sleep at night)](https://ff1959.wordpress.com/2013/07/31/ldap-hardening-server-security-so-administrators-can-sleep-at-night/)
- [LDAP Authentication Best Practices](http://web.archive.org/web/20130801091446/http://www.ldapguru.info/ldap/authentication-best-practices.html) - retrieved from web.archive.org
- [Hardening OpenLDAP on Linux with AppArmor and systemd](http://www.openldap.org/conf/odd-tuebingen-2018/Michael1.pdf) - slides
- [zytrax LDAP for Rocket Scientists - LDAP Security](http://www.zytrax.com/books/ldap/ch15/)
- [How To Encrypt OpenLDAP Connections Using STARTTLS](https://www.digitalocean.com/community/tutorials/how-to-encrypt-openldap-connections-using-starttls)

### DNS

- [NIST SP 800-81-2 - Secure Domain Name System (DNS) Deployment Guide](https://csrc.nist.gov/publications/detail/sp/800-81/2/final) (2013)
- [CMU SEI - Six Best Practices for Securing a Robust Domain Name System (DNS) Infrastructure](https://insights.sei.cmu.edu/sei_blog/2017/02/six-best-practices-for-securing-a-robust-domain-name-system-dns-infrastructure.html)
- [NSA BIND 9 DNS Security](https://apps.nsa.gov/iaarchive/library/ia-guidance/security-configuration/applications/bind-9-dns-security.cfm) (2011)

### NTP

- [IETF - Network Time Protocol Best Current Practices draft-ietf-ntp-bcp](https://tools.ietf.org/html/draft-reilly-ntp-bcp) (2019)
- [CMU SEI - Best Practices for NTP Services](https://insights.sei.cmu.edu/sei_blog/2017/04/best-practices-for-ntp-services.html)
- [Linux.com - Arrive On Time With NTP -- Part 2: Security Options](https://www.linux.com/learn/arrive-time-ntp-part-2-security-options)
- [Linux.com - Arrive On Time With NTP -- Part 3: Secure Setup](https://www.linux.com/learn/2017/2/arrive-time-ntp-part-3-secure-setup)

### NFS

- [Linux NFS-HOWTO - Security and NFS](https://www.tldp.org/HOWTO/NFS-HOWTO/security.html) - a good overview of NFS security issues and some mitigations
- [Red Hat - A Guide to Securing Red Hat Enterprise Linux 7 - Securing NFS](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html-single/security_guide/index#sec-Securing_NFS)
- [Red Hat - RHEL7 Storage Administration Guide - Securing NFS](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/storage_administration_guide/s1-nfs-security)
- [NFSv4 without Kerberos and permissions](https://lists.debian.org/debian-user/2017/10/msg00476.html) - why NFSv4 without Kerberos does not provide security
- [CertDepot - RHEL7: Use Kerberos to control access to NFS network shares](https://www.certdepot.net/rhel7-use-kerberos-control-access-nfs-network-shares/)

### CUPS

- [CUPS Server Security](https://www.cups.org/doc/security.html)

## Authentication - Passwords

- [UK NCSC - Password administration for system owners](https://www.ncsc.gov.uk/collection/passwords)
- [NIST SP 800-63 Digital Identity Guidelines](https://pages.nist.gov/800-63-3/)

## Hardware - BIOS - UEFI

- [NSA Info Sheet: UEFI Lockdown Quick Guidance (March 2018)](https://www.nsa.gov/Portals/70/documents/what-we-do/cybersecurity/professional-resources/csi-uefi-lockdown.pdf?v=1)
- [NSA Tech Report: UEFI Defensive Practices Guidance (July 2017)](https://www.nsa.gov/Portals/70/documents/what-we-do/cybersecurity/professional-resources/ctr-uefi-defensive-practices-guidance.pdf?ver=2018-11-06-074836-090)

## Cloud

- [NSA Info Sheet: Cloud Security Basics (August 2018)](https://www.nsa.gov/Portals/70/documents/what-we-do/cybersecurity/professional-resources/csi-cloud-security-basics.pdf?v=1)
- [DISA DoD Cloud Computing Security](https://iase.disa.mil/cloud_security/Pages/index.aspx)

# Tools

## Tools to check security hardening

### GNU/Linux

- [Lynis](https://cisofy.com/lynis/) - script to check the configuration of Linux hosts
- [OpenSCAP Base](https://www.open-scap.org/tools/openscap-base/) - oscap command line tool
- [SCAP Workbench](https://www.open-scap.org/tools/scap-workbench/) - GUI for oscap
- [Tiger - The Unix security audit and intrusion detection tool](https://www.nongnu.org/tiger/) (might be outdated)

### Network Devices

- [Nipper-ng](https://github.com/arpitn30/nipper-ng) - to check the configuration of network devices (does not seem to be updated)

### TLS/SSL

- [Qualys SSL Labs - List of tools to assess TLS/SSL servers and clients](https://github.com/ssllabs/research/wiki/Assessment-Tools)

### Docker

- [Docker Bench for Security](https://github.com/docker/docker-bench-security) - script that checks for dozens of common best-practices around deploying Docker containers in production, inspired by the CIS Docker Community Edition Benchmark v1.1.0.

## Tools to apply security hardening

### GNU/Linux

- [Linux Server Hardener](https://github.com/pratiktri/server_init_harden) - for Debian/Ubuntu (2019)
- [Bastille Linux](http://bastille-linux.sourceforge.net/) - outdated

### Windows

- [Hardentools](https://github.com/securitywithoutborders/hardentools) - for Windows individual users (not corporate environments) at risk, who might want an extra level of security at the price of some usability.
- [Windows 10 Hardening](https://github.com/aghorler/Windows-10-Hardening) - A collective resource of settings modifications (mostly opt-outs) that attempt to make Windows 10 as private and as secure as possible.
- [Hardening Auditor](https://github.com/cottinghamd/HardeningAuditor) - Scripts for comparing Microsoft Windows compliance with the ASD 1709 & Office 2016 Hardening Guides
- [Windows 10 Initial Setup Script](https://github.com/Disassembler0/Win10-Initial-Setup-Script) - PowerShell script for automation of routine tasks done after fresh installations of Windows 10 / Server 2016 / Server 2019


# Books

# Other Awesome Lists

(borrowed from [Awesome Security](https://github.com/sbilly/awesome-security))

## Other Awesome Security Lists

- [Awesome Security](https://github.com/sbilly/awesome-security) - A collection of awesome software, libraries, documents, books, resources and cools stuffs about security.
- [Android Security Awesome](https://github.com/ashishb/android-security-awesome) - A collection of android security related resources.
- [Awesome CTF](https://github.com/apsdehal/awesome-ctf) - A curated list of CTF frameworks, libraries, resources and software.
- [Awesome Cyber Skills](https://github.com/joe-shenouda/awesome-cyber-skills) - A curated list of hacking environments where you can train your cyber skills legally and safely.
- [Awesome Hacking](https://github.com/carpedm20/awesome-hacking) - A curated list of awesome Hacking tutorials, tools and resources.
- [Awesome Honeypots](https://github.com/paralax/awesome-honeypots) - An awesome list of honeypot resources.
- [Awesome Malware Analysis](https://github.com/rshipp/awesome-malware-analysis) - A curated list of awesome malware analysis tools and resources.
- [Awesome PCAP Tools](https://github.com/caesar0301/awesome-pcaptools) - A collection of tools developed by other researchers in the Computer Science area to process network traces.
- [Awesome Pentest](https://github.com/enaqx/awesome-pentest) - A collection of awesome penetration testing resources, tools and other shiny things.
- [Awesome Linux Containers](https://github.com/Friz-zy/awesome-linux-containers) - A curated list of awesome Linux Containers frameworks, libraries and software.
- [Awesome Incident Response](https://github.com/meirwah/awesome-incident-response) - A curated list of resources for incident response.
- [Awesome Web Hacking](https://github.com/infoslack/awesome-web-hacking) - This list is for anyone wishing to learn about web application security but do not have a starting point.
- [Awesome Threat Intelligence](https://github.com/hslatman/awesome-threat-intelligence) - A curated list of threat intelligence resources.
- [Awesome Pentest Cheat Sheets](https://github.com/coreb1t/awesome-pentest-cheat-sheets) - Collection of the cheat sheets useful for pentesting
- [Awesome Industrial Control System Security](https://github.com/mpesen/awesome-industrial-control-system-security) - A curated list of resources related to Industrial Control System (ICS) security.
- [Awesome YARA](https://github.com/InQuest/awesome-yara) - A curated list of awesome YARA rules, tools, and people.
- [Awesome Threat Detection and Hunting](https://github.com/0x4D31/awesome-threat-detection) - A curated list of awesome threat detection and hunting resources.
- [Awesome Container Security](https://github.com/kai5263499/container-security-awesome) - A curated list of awesome resources related to container building and runtime security
- [Awesome Crypto Papers](https://github.com/pFarb/awesome-crypto-papers) - A curated list of cryptography papers, articles, tutorials and howtos.

