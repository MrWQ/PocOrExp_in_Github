## CVE-2017-1001004
 typed-function before 0.10.6 had an arbitrary code execution in the JavaScript engine. Creating a typed function with JavaScript code in the name could result arbitrary execution.



- [https://github.com/ossf-cve-benchmark/CVE-2017-1001004](https://github.com/ossf-cve-benchmark/CVE-2017-1001004) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-1001004.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-1001004.svg)

## CVE-2017-1000405
 The Linux Kernel versions 2.6.38 through 4.14 have a problematic use of pmd_mkdirty() in the touch_pmd() function inside the THP implementation. touch_pmd() can be reached by get_user_pages(). In such case, the pmd will become dirty. This scenario breaks the new can_follow_write_pmd()'s logic - pmd can become dirty without going through a COW cycle. This bug is not as severe as the original "Dirty cow" because an ext4 file (or any other regular file) cannot be mapped using THP. Nevertheless, it does allow us to overwrite read-only huge pages. For example, the zero huge page and sealed shmem files can be overwritten (since their mapping can be populated using THP). Note that after the first write page-fault to the zero page, it will be replaced with a new fresh (and zeroed) thp.



- [https://github.com/bindecy/HugeDirtyCowPOC](https://github.com/bindecy/HugeDirtyCowPOC) :  ![starts](https://img.shields.io/github/stars/bindecy/HugeDirtyCowPOC.svg) ![forks](https://img.shields.io/github/forks/bindecy/HugeDirtyCowPOC.svg)

## CVE-2017-1000367
 Todd Miller's sudo version 1.8.20 and earlier is vulnerable to an input validation (embedded spaces) in the get_process_ttyname() function resulting in information disclosure and command execution.



- [https://github.com/Al1ex/LinuxEelvation](https://github.com/Al1ex/LinuxEelvation) :  ![starts](https://img.shields.io/github/stars/Al1ex/LinuxEelvation.svg) ![forks](https://img.shields.io/github/forks/Al1ex/LinuxEelvation.svg)

- [https://github.com/c0d3z3r0/sudo-CVE-2017-1000367](https://github.com/c0d3z3r0/sudo-CVE-2017-1000367) :  ![starts](https://img.shields.io/github/stars/c0d3z3r0/sudo-CVE-2017-1000367.svg) ![forks](https://img.shields.io/github/forks/c0d3z3r0/sudo-CVE-2017-1000367.svg)

- [https://github.com/pucerpocok/sudo_exploit](https://github.com/pucerpocok/sudo_exploit) :  ![starts](https://img.shields.io/github/stars/pucerpocok/sudo_exploit.svg) ![forks](https://img.shields.io/github/forks/pucerpocok/sudo_exploit.svg)

- [https://github.com/homjxi0e/CVE-2017-1000367](https://github.com/homjxi0e/CVE-2017-1000367) :  ![starts](https://img.shields.io/github/stars/homjxi0e/CVE-2017-1000367.svg) ![forks](https://img.shields.io/github/forks/homjxi0e/CVE-2017-1000367.svg)

- [https://github.com/letsr00t/CVE-2017-1000367](https://github.com/letsr00t/CVE-2017-1000367) :  ![starts](https://img.shields.io/github/stars/letsr00t/CVE-2017-1000367.svg) ![forks](https://img.shields.io/github/forks/letsr00t/CVE-2017-1000367.svg)

## CVE-2017-1000117
 A malicious third-party can give a crafted "ssh://..." URL to an unsuspecting victim, and an attempt to visit the URL can result in any program that exists on the victim's machine being executed. Such a URL could be placed in the .gitmodules file of a malicious project, and an unsuspecting victim could be tricked into running "git clone --recurse-submodules" to trigger the vulnerability.



- [https://github.com/greymd/CVE-2017-1000117](https://github.com/greymd/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/greymd/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/greymd/CVE-2017-1000117.svg)

- [https://github.com/Manouchehri/CVE-2017-1000117](https://github.com/Manouchehri/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/Manouchehri/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/Manouchehri/CVE-2017-1000117.svg)

- [https://github.com/timwr/CVE-2017-1000117](https://github.com/timwr/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/timwr/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/timwr/CVE-2017-1000117.svg)

- [https://github.com/ieee0824/CVE-2017-1000117](https://github.com/ieee0824/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/ieee0824/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/ieee0824/CVE-2017-1000117.svg)

- [https://github.com/VulApps/CVE-2017-1000117](https://github.com/VulApps/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/VulApps/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/VulApps/CVE-2017-1000117.svg)

- [https://github.com/AnonymKing/CVE-2017-1000117](https://github.com/AnonymKing/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/AnonymKing/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/AnonymKing/CVE-2017-1000117.svg)

- [https://github.com/nkoneko/CVE-2017-1000117](https://github.com/nkoneko/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/nkoneko/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/nkoneko/CVE-2017-1000117.svg)

- [https://github.com/leezp/CVE-2017-1000117](https://github.com/leezp/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/leezp/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/leezp/CVE-2017-1000117.svg)

- [https://github.com/sasairc/CVE-2017-1000117_wasawasa](https://github.com/sasairc/CVE-2017-1000117_wasawasa) :  ![starts](https://img.shields.io/github/stars/sasairc/CVE-2017-1000117_wasawasa.svg) ![forks](https://img.shields.io/github/forks/sasairc/CVE-2017-1000117_wasawasa.svg)

- [https://github.com/rootclay/CVE-2017-1000117](https://github.com/rootclay/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/rootclay/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/rootclay/CVE-2017-1000117.svg)

- [https://github.com/cved-sources/cve-2017-1000117](https://github.com/cved-sources/cve-2017-1000117) :  ![starts](https://img.shields.io/github/stars/cved-sources/cve-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/cved-sources/cve-2017-1000117.svg)

- [https://github.com/chenzhuo0618/test](https://github.com/chenzhuo0618/test) :  ![starts](https://img.shields.io/github/stars/chenzhuo0618/test.svg) ![forks](https://img.shields.io/github/forks/chenzhuo0618/test.svg)

- [https://github.com/ieee0824/CVE-2017-1000117-sl](https://github.com/ieee0824/CVE-2017-1000117-sl) :  ![starts](https://img.shields.io/github/stars/ieee0824/CVE-2017-1000117-sl.svg) ![forks](https://img.shields.io/github/forks/ieee0824/CVE-2017-1000117-sl.svg)

- [https://github.com/alilangtest/CVE-2017-1000117](https://github.com/alilangtest/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/alilangtest/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/alilangtest/CVE-2017-1000117.svg)

- [https://github.com/takehaya/CVE-2017-1000117](https://github.com/takehaya/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/takehaya/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/takehaya/CVE-2017-1000117.svg)

- [https://github.com/Jerry-zhuang/CVE-2017-1000117](https://github.com/Jerry-zhuang/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/Jerry-zhuang/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/Jerry-zhuang/CVE-2017-1000117.svg)

- [https://github.com/chu1337/CVE-2017-1000117](https://github.com/chu1337/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/chu1337/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/chu1337/CVE-2017-1000117.svg)

- [https://github.com/Shadow5523/CVE-2017-1000117-test](https://github.com/Shadow5523/CVE-2017-1000117-test) :  ![starts](https://img.shields.io/github/stars/Shadow5523/CVE-2017-1000117-test.svg) ![forks](https://img.shields.io/github/forks/Shadow5523/CVE-2017-1000117-test.svg)

- [https://github.com/thelastbyte/CVE-2017-1000117](https://github.com/thelastbyte/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/thelastbyte/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/thelastbyte/CVE-2017-1000117.svg)

- [https://github.com/siling2017/CVE-2017-1000117](https://github.com/siling2017/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/siling2017/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/siling2017/CVE-2017-1000117.svg)

- [https://github.com/ikmski/CVE-2017-1000117](https://github.com/ikmski/CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/ikmski/CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/ikmski/CVE-2017-1000117.svg)

- [https://github.com/shogo82148/Fix-CVE-2017-1000117](https://github.com/shogo82148/Fix-CVE-2017-1000117) :  ![starts](https://img.shields.io/github/stars/shogo82148/Fix-CVE-2017-1000117.svg) ![forks](https://img.shields.io/github/forks/shogo82148/Fix-CVE-2017-1000117.svg)

## CVE-2017-1000112
 Linux kernel: Exploitable memory corruption due to UFO to non-UFO path switch. When building a UFO packet with MSG_MORE __ip_append_data() calls ip_ufo_append_data() to append. However in between two send() calls, the append path can be switched from UFO to non-UFO one, which leads to a memory corruption. In case UFO packet lengths exceeds MTU, copy = maxfraglen - skb-len becomes negative on the non-UFO path and the branch to allocate new skb is taken. This triggers fragmentation and computation of fraggap = skb_prev-len - maxfraglen. Fraggap can exceed MTU, causing copy = datalen - transhdrlen - fraggap to become negative. Subsequently skb_copy_and_csum_bits() writes out-of-bounds. A similar issue is present in IPv6 code. The bug was introduced in e89e9cf539a2 ("[IPv4/IPv6]: UFO Scatter-gather approach") on Oct 18 2005.



- [https://github.com/Al1ex/LinuxEelvation](https://github.com/Al1ex/LinuxEelvation) :  ![starts](https://img.shields.io/github/stars/Al1ex/LinuxEelvation.svg) ![forks](https://img.shields.io/github/forks/Al1ex/LinuxEelvation.svg)

- [https://github.com/ol0273st-s/CVE-2017-1000112-Adpated](https://github.com/ol0273st-s/CVE-2017-1000112-Adpated) :  ![starts](https://img.shields.io/github/stars/ol0273st-s/CVE-2017-1000112-Adpated.svg) ![forks](https://img.shields.io/github/forks/ol0273st-s/CVE-2017-1000112-Adpated.svg)

- [https://github.com/IT19083124/SNP-Assignment](https://github.com/IT19083124/SNP-Assignment) :  ![starts](https://img.shields.io/github/stars/IT19083124/SNP-Assignment.svg) ![forks](https://img.shields.io/github/forks/IT19083124/SNP-Assignment.svg)

- [https://github.com/Spydomain/CVE-2017-1000112-PoC](https://github.com/Spydomain/CVE-2017-1000112-PoC) :  ![starts](https://img.shields.io/github/stars/Spydomain/CVE-2017-1000112-PoC.svg) ![forks](https://img.shields.io/github/forks/Spydomain/CVE-2017-1000112-PoC.svg)

- [https://github.com/hikame/docker_escape_pwn](https://github.com/hikame/docker_escape_pwn) :  ![starts](https://img.shields.io/github/stars/hikame/docker_escape_pwn.svg) ![forks](https://img.shields.io/github/forks/hikame/docker_escape_pwn.svg)

## CVE-2017-1000083
 backend/comics/comics-document.c (aka the comic book backend) in GNOME Evince before 3.24.1 allows remote attackers to execute arbitrary commands via a .cbt file that is a TAR archive containing a filename beginning with a "--" command-line option substring, as demonstrated by a --checkpoint-action=exec=bash at the beginning of the filename.



- [https://github.com/matlink/evince-cve-2017-1000083](https://github.com/matlink/evince-cve-2017-1000083) :  ![starts](https://img.shields.io/github/stars/matlink/evince-cve-2017-1000083.svg) ![forks](https://img.shields.io/github/forks/matlink/evince-cve-2017-1000083.svg)

- [https://github.com/matlink/cve-2017-1000083-atril-nautilus](https://github.com/matlink/cve-2017-1000083-atril-nautilus) :  ![starts](https://img.shields.io/github/stars/matlink/cve-2017-1000083-atril-nautilus.svg) ![forks](https://img.shields.io/github/forks/matlink/cve-2017-1000083-atril-nautilus.svg)

## CVE-2017-18354
 Rendertron 1.0.0 allows for alternative protocols such as 'file://' introducing a Local File Inclusion (LFI) bug where arbitrary files can be read by a remote attacker.



- [https://github.com/CQ-Tools/CVE-2017-18354-unfixed](https://github.com/CQ-Tools/CVE-2017-18354-unfixed) :  ![starts](https://img.shields.io/github/stars/CQ-Tools/CVE-2017-18354-unfixed.svg) ![forks](https://img.shields.io/github/forks/CQ-Tools/CVE-2017-18354-unfixed.svg)

- [https://github.com/CQ-Tools/CVE-2017-18354-fixed](https://github.com/CQ-Tools/CVE-2017-18354-fixed) :  ![starts](https://img.shields.io/github/stars/CQ-Tools/CVE-2017-18354-fixed.svg) ![forks](https://img.shields.io/github/forks/CQ-Tools/CVE-2017-18354-fixed.svg)

- [https://github.com/ossf-cve-benchmark/CVE-2017-18354](https://github.com/ossf-cve-benchmark/CVE-2017-18354) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-18354.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-18354.svg)

## CVE-2017-18344
 The timer_create syscall implementation in kernel/time/posix-timers.c in the Linux kernel before 4.14.8 doesn't properly validate the sigevent-sigev_notify field, which leads to out-of-bounds access in the show_timer function (called when /proc/$PID/timers is read). This allows userspace applications to read arbitrary kernel memory (on a kernel built with CONFIG_POSIX_TIMERS and CONFIG_CHECKPOINT_RESTORE).



- [https://github.com/echo-devim/exploit_linux_kernel4.13](https://github.com/echo-devim/exploit_linux_kernel4.13) :  ![starts](https://img.shields.io/github/stars/echo-devim/exploit_linux_kernel4.13.svg) ![forks](https://img.shields.io/github/forks/echo-devim/exploit_linux_kernel4.13.svg)

- [https://github.com/hikame/docker_escape_pwn](https://github.com/hikame/docker_escape_pwn) :  ![starts](https://img.shields.io/github/stars/hikame/docker_escape_pwn.svg) ![forks](https://img.shields.io/github/forks/hikame/docker_escape_pwn.svg)

## CVE-2017-18019
 In K7 Total Security before 15.1.0.305, user-controlled input to the K7Sentry device is not sufficiently sanitized: the user-controlled input can be used to compare an arbitrary memory address with a fixed value, which in turn can be used to read the contents of arbitrary memory. Similarly, the product crashes upon a \\.\K7Sentry DeviceIoControl call with an invalid kernel pointer.



- [https://github.com/SpiralBL0CK/CVE-2017-18019](https://github.com/SpiralBL0CK/CVE-2017-18019) :  ![starts](https://img.shields.io/github/stars/SpiralBL0CK/CVE-2017-18019.svg) ![forks](https://img.shields.io/github/forks/SpiralBL0CK/CVE-2017-18019.svg)

## CVE-2017-17692
 Samsung Internet Browser 5.4.02.3 allows remote attackers to bypass the Same Origin Policy and obtain sensitive information via crafted JavaScript code that redirects to a child tab and rewrites the innerHTML property.



- [https://github.com/specloli/CVE-2017-17692](https://github.com/specloli/CVE-2017-17692) :  ![starts](https://img.shields.io/github/stars/specloli/CVE-2017-17692.svg) ![forks](https://img.shields.io/github/forks/specloli/CVE-2017-17692.svg)

## CVE-2017-17562
 Embedthis GoAhead before 3.6.5 allows remote code execution if CGI is enabled and a CGI program is dynamically linked. This is a result of initializing the environment of forked CGI scripts using untrusted HTTP request parameters in the cgiHandler function in cgi.c. When combined with the glibc dynamic linker, this behaviour can be abused for remote code execution using special parameter names such as LD_PRELOAD. An attacker can POST their shared object payload in the body of the request, and reference it using /proc/self/fd/0.



- [https://github.com/ivanitlearning/CVE-2017-17562](https://github.com/ivanitlearning/CVE-2017-17562) :  ![starts](https://img.shields.io/github/stars/ivanitlearning/CVE-2017-17562.svg) ![forks](https://img.shields.io/github/forks/ivanitlearning/CVE-2017-17562.svg)

- [https://github.com/nu11pointer/goahead-rce-exploit](https://github.com/nu11pointer/goahead-rce-exploit) :  ![starts](https://img.shields.io/github/stars/nu11pointer/goahead-rce-exploit.svg) ![forks](https://img.shields.io/github/forks/nu11pointer/goahead-rce-exploit.svg)

- [https://github.com/1337g/CVE-2017-17562](https://github.com/1337g/CVE-2017-17562) :  ![starts](https://img.shields.io/github/stars/1337g/CVE-2017-17562.svg) ![forks](https://img.shields.io/github/forks/1337g/CVE-2017-17562.svg)

- [https://github.com/joaomagfreitas/bash-CVE-2017-17562](https://github.com/joaomagfreitas/bash-CVE-2017-17562) :  ![starts](https://img.shields.io/github/stars/joaomagfreitas/bash-CVE-2017-17562.svg) ![forks](https://img.shields.io/github/forks/joaomagfreitas/bash-CVE-2017-17562.svg)

- [https://github.com/crispy-peppers/Goahead-CVE-2017-17562](https://github.com/crispy-peppers/Goahead-CVE-2017-17562) :  ![starts](https://img.shields.io/github/stars/crispy-peppers/Goahead-CVE-2017-17562.svg) ![forks](https://img.shields.io/github/forks/crispy-peppers/Goahead-CVE-2017-17562.svg)

- [https://github.com/cyberharsh/GoAhead-cve---2017--17562](https://github.com/cyberharsh/GoAhead-cve---2017--17562) :  ![starts](https://img.shields.io/github/stars/cyberharsh/GoAhead-cve---2017--17562.svg) ![forks](https://img.shields.io/github/forks/cyberharsh/GoAhead-cve---2017--17562.svg)

## CVE-2017-17099
 There exists an unauthenticated SEH based Buffer Overflow vulnerability in the HTTP server of Flexense SyncBreeze Enterprise v10.1.16. When sending a GET request with an excessive length, it is possible for a malicious user to overwrite the SEH record and execute a payload that would run under the Windows SYSTEM account.



- [https://github.com/wetw0rk/Exploit-Development](https://github.com/wetw0rk/Exploit-Development) :  ![starts](https://img.shields.io/github/stars/wetw0rk/Exploit-Development.svg) ![forks](https://img.shields.io/github/forks/wetw0rk/Exploit-Development.svg)

## CVE-2017-16995
 The check_alu_op function in kernel/bpf/verifier.c in the Linux kernel through 4.4 allows local users to cause a denial of service (memory corruption) or possibly have unspecified other impact by leveraging incorrect sign extension.



- [https://github.com/Al1ex/LinuxEelvation](https://github.com/Al1ex/LinuxEelvation) :  ![starts](https://img.shields.io/github/stars/Al1ex/LinuxEelvation.svg) ![forks](https://img.shields.io/github/forks/Al1ex/LinuxEelvation.svg)

- [https://github.com/Al1ex/CVE-2017-16995](https://github.com/Al1ex/CVE-2017-16995) :  ![starts](https://img.shields.io/github/stars/Al1ex/CVE-2017-16995.svg) ![forks](https://img.shields.io/github/forks/Al1ex/CVE-2017-16995.svg)

- [https://github.com/dangokyo/CVE_2017_16995](https://github.com/dangokyo/CVE_2017_16995) :  ![starts](https://img.shields.io/github/stars/dangokyo/CVE_2017_16995.svg) ![forks](https://img.shields.io/github/forks/dangokyo/CVE_2017_16995.svg)

- [https://github.com/ph4ntonn/CVE-2017-16995](https://github.com/ph4ntonn/CVE-2017-16995) :  ![starts](https://img.shields.io/github/stars/ph4ntonn/CVE-2017-16995.svg) ![forks](https://img.shields.io/github/forks/ph4ntonn/CVE-2017-16995.svg)

- [https://github.com/gugronnier/CVE-2017-16995](https://github.com/gugronnier/CVE-2017-16995) :  ![starts](https://img.shields.io/github/stars/gugronnier/CVE-2017-16995.svg) ![forks](https://img.shields.io/github/forks/gugronnier/CVE-2017-16995.svg)

- [https://github.com/vnik5287/CVE-2017-16995](https://github.com/vnik5287/CVE-2017-16995) :  ![starts](https://img.shields.io/github/stars/vnik5287/CVE-2017-16995.svg) ![forks](https://img.shields.io/github/forks/vnik5287/CVE-2017-16995.svg)

- [https://github.com/littlebin404/CVE-2017-16995](https://github.com/littlebin404/CVE-2017-16995) :  ![starts](https://img.shields.io/github/stars/littlebin404/CVE-2017-16995.svg) ![forks](https://img.shields.io/github/forks/littlebin404/CVE-2017-16995.svg)

- [https://github.com/senyuuri/cve-2017-16995](https://github.com/senyuuri/cve-2017-16995) :  ![starts](https://img.shields.io/github/stars/senyuuri/cve-2017-16995.svg) ![forks](https://img.shields.io/github/forks/senyuuri/cve-2017-16995.svg)

- [https://github.com/C0dak/CVE-2017-16995](https://github.com/C0dak/CVE-2017-16995) :  ![starts](https://img.shields.io/github/stars/C0dak/CVE-2017-16995.svg) ![forks](https://img.shields.io/github/forks/C0dak/CVE-2017-16995.svg)

- [https://github.com/anldori/CVE-2017-16995](https://github.com/anldori/CVE-2017-16995) :  ![starts](https://img.shields.io/github/stars/anldori/CVE-2017-16995.svg) ![forks](https://img.shields.io/github/forks/anldori/CVE-2017-16995.svg)

- [https://github.com/mareks1007/cve-2017-16995](https://github.com/mareks1007/cve-2017-16995) :  ![starts](https://img.shields.io/github/stars/mareks1007/cve-2017-16995.svg) ![forks](https://img.shields.io/github/forks/mareks1007/cve-2017-16995.svg)

- [https://github.com/fei9747/CVE-2017-16995](https://github.com/fei9747/CVE-2017-16995) :  ![starts](https://img.shields.io/github/stars/fei9747/CVE-2017-16995.svg) ![forks](https://img.shields.io/github/forks/fei9747/CVE-2017-16995.svg)

- [https://github.com/ZhiQiAnSecFork/cve-2017-16995](https://github.com/ZhiQiAnSecFork/cve-2017-16995) :  ![starts](https://img.shields.io/github/stars/ZhiQiAnSecFork/cve-2017-16995.svg) ![forks](https://img.shields.io/github/forks/ZhiQiAnSecFork/cve-2017-16995.svg)

- [https://github.com/xxxTectationxxx/CVE-2017-16995](https://github.com/xxxTectationxxx/CVE-2017-16995) :  ![starts](https://img.shields.io/github/stars/xxxTectationxxx/CVE-2017-16995.svg) ![forks](https://img.shields.io/github/forks/xxxTectationxxx/CVE-2017-16995.svg)

- [https://github.com/ivilpez/cve-2017-16995.c](https://github.com/ivilpez/cve-2017-16995.c) :  ![starts](https://img.shields.io/github/stars/ivilpez/cve-2017-16995.c.svg) ![forks](https://img.shields.io/github/forks/ivilpez/cve-2017-16995.c.svg)

- [https://github.com/Lumindu/CVE-2017-16995-Linux-Kernel---BPF-Sign-Extension-Local-Privilege-Escalation-](https://github.com/Lumindu/CVE-2017-16995-Linux-Kernel---BPF-Sign-Extension-Local-Privilege-Escalation-) :  ![starts](https://img.shields.io/github/stars/Lumindu/CVE-2017-16995-Linux-Kernel---BPF-Sign-Extension-Local-Privilege-Escalation-.svg) ![forks](https://img.shields.io/github/forks/Lumindu/CVE-2017-16995-Linux-Kernel---BPF-Sign-Extension-Local-Privilege-Escalation-.svg)

## CVE-2017-16939
 The XFRM dump policy implementation in net/xfrm/xfrm_user.c in the Linux kernel before 4.13.11 allows local users to gain privileges or cause a denial of service (use-after-free) via a crafted SO_RCVBUF setsockopt system call in conjunction with XFRM_MSG_GETPOLICY Netlink messages.



- [https://github.com/Al1ex/LinuxEelvation](https://github.com/Al1ex/LinuxEelvation) :  ![starts](https://img.shields.io/github/stars/Al1ex/LinuxEelvation.svg) ![forks](https://img.shields.io/github/forks/Al1ex/LinuxEelvation.svg)

## CVE-2017-16930
 The remote management interface on the Claymore Dual GPU miner 10.1 allows an unauthenticated remote attacker to execute arbitrary code due to a stack-based buffer overflow in the request handler. This can be exploited via a long API request that is mishandled during logging.



- [https://github.com/tintinweb/pub](https://github.com/tintinweb/pub) :  ![starts](https://img.shields.io/github/stars/tintinweb/pub.svg) ![forks](https://img.shields.io/github/forks/tintinweb/pub.svg)

## CVE-2017-16877
 ZEIT Next.js before 2.4.1 has directory traversal under the /_next and /static request namespace, allowing attackers to obtain sensitive information.



- [https://github.com/ossf-cve-benchmark/CVE-2017-16877](https://github.com/ossf-cve-benchmark/CVE-2017-16877) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16877.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16877.svg)

## CVE-2017-16806
 The Process function in RemoteTaskServer/WebServer/HttpServer.cs in Ulterius before 1.9.5.0 allows HTTP server directory traversal.



- [https://github.com/rickoooooo/ulteriusExploit](https://github.com/rickoooooo/ulteriusExploit) :  ![starts](https://img.shields.io/github/stars/rickoooooo/ulteriusExploit.svg) ![forks](https://img.shields.io/github/forks/rickoooooo/ulteriusExploit.svg)

## CVE-2017-16778
 An access control weakness in the DTMF tone receiver of Fermax Outdoor Panel allows physical attackers to inject a Dual-Tone-Multi-Frequency (DTMF) tone to invoke an access grant that would allow physical access to a restricted floor/level. By design, only a residential unit owner may allow such an access grant. However, due to incorrect access control, an attacker could inject it via the speaker unit to perform an access grant to gain unauthorized access, as demonstrated by a loud DTMF tone representing '1' and a long '#' (697 Hz and 1209 Hz, followed by 941 Hz and 1477 Hz).



- [https://github.com/breaktoprotect/CVE-2017-16778-Intercom-DTMF-Injection](https://github.com/breaktoprotect/CVE-2017-16778-Intercom-DTMF-Injection) :  ![starts](https://img.shields.io/github/stars/breaktoprotect/CVE-2017-16778-Intercom-DTMF-Injection.svg) ![forks](https://img.shields.io/github/forks/breaktoprotect/CVE-2017-16778-Intercom-DTMF-Injection.svg)

## CVE-2017-16748
 An attacker can log into the local Niagara platform (Niagara AX Framework Versions 3.8 and prior or Niagara 4 Framework Versions 4.4 and prior) using a disabled account name and a blank password, granting the attacker administrator access to the Niagara system.



- [https://github.com/GainSec/CVE-2017-16744-and-CVE-2017-16748-Tridium-Niagara](https://github.com/GainSec/CVE-2017-16744-and-CVE-2017-16748-Tridium-Niagara) :  ![starts](https://img.shields.io/github/stars/GainSec/CVE-2017-16744-and-CVE-2017-16748-Tridium-Niagara.svg) ![forks](https://img.shields.io/github/forks/GainSec/CVE-2017-16744-and-CVE-2017-16748-Tridium-Niagara.svg)

## CVE-2017-16695
 ** RESERVED ** This candidate has been reserved by an organization or individual that will use it when announcing a new security problem.  When the candidate has been publicized, the details for this candidate will be provided.



- [https://github.com/Jewel591/Privilege-Escalation](https://github.com/Jewel591/Privilege-Escalation) :  ![starts](https://img.shields.io/github/stars/Jewel591/Privilege-Escalation.svg) ![forks](https://img.shields.io/github/forks/Jewel591/Privilege-Escalation.svg)

## CVE-2017-16651
 Roundcube Webmail before 1.1.10, 1.2.x before 1.2.7, and 1.3.x before 1.3.3 allows unauthorized access to arbitrary files on the host's filesystem, including configuration files, as exploited in the wild in November 2017. The attacker must be able to authenticate at the target system with a valid username/password as the attack requires an active session. The issue is related to file-based attachment plugins and _task=settings&_action=upload-display&_from=timezone requests.



- [https://github.com/starnightcyber/Exploit-Database-For-Webmail](https://github.com/starnightcyber/Exploit-Database-For-Webmail) :  ![starts](https://img.shields.io/github/stars/starnightcyber/Exploit-Database-For-Webmail.svg) ![forks](https://img.shields.io/github/forks/starnightcyber/Exploit-Database-For-Webmail.svg)

- [https://github.com/ropbear/CVE-2017-16651](https://github.com/ropbear/CVE-2017-16651) :  ![starts](https://img.shields.io/github/stars/ropbear/CVE-2017-16651.svg) ![forks](https://img.shields.io/github/forks/ropbear/CVE-2017-16651.svg)

## CVE-2017-16245
 ** RESERVED ** This candidate has been reserved by an organization or individual that will use it when announcing a new security problem.  When the candidate has been publicized, the details for this candidate will be provided.



- [https://github.com/AOCorsaire/CVE-2017-16245](https://github.com/AOCorsaire/CVE-2017-16245) :  ![starts](https://img.shields.io/github/stars/AOCorsaire/CVE-2017-16245.svg) ![forks](https://img.shields.io/github/forks/AOCorsaire/CVE-2017-16245.svg)

## CVE-2017-16226
 The static-eval module is intended to evaluate statically-analyzable expressions. In affected versions, untrusted user input is able to access the global function constructor, effectively allowing arbitrary code execution.



- [https://github.com/ossf-cve-benchmark/CVE-2017-16226](https://github.com/ossf-cve-benchmark/CVE-2017-16226) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16226.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16226.svg)

## CVE-2017-16136
 method-override is a module used by the Express.js framework to let you use HTTP verbs such as PUT or DELETE in places where the client doesn't support it. method-override is vulnerable to a regular expression denial of service vulnerability when specially crafted input is passed in to be parsed via the X-HTTP-Method-Override header.



- [https://github.com/CQ-Tools/CVE-2017-16136-unfixed](https://github.com/CQ-Tools/CVE-2017-16136-unfixed) :  ![starts](https://img.shields.io/github/stars/CQ-Tools/CVE-2017-16136-unfixed.svg) ![forks](https://img.shields.io/github/forks/CQ-Tools/CVE-2017-16136-unfixed.svg)

- [https://github.com/CQ-Tools/CVE-2017-16136-fixed](https://github.com/CQ-Tools/CVE-2017-16136-fixed) :  ![starts](https://img.shields.io/github/stars/CQ-Tools/CVE-2017-16136-fixed.svg) ![forks](https://img.shields.io/github/forks/CQ-Tools/CVE-2017-16136-fixed.svg)

- [https://github.com/ossf-cve-benchmark/CVE-2017-16136](https://github.com/ossf-cve-benchmark/CVE-2017-16136) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16136.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16136.svg)

## CVE-2017-16114
 The marked module is vulnerable to a regular expression denial of service. Based on the information published in the public issue, 1k characters can block for around 6 seconds.



- [https://github.com/ossf-cve-benchmark/CVE-2017-16114](https://github.com/ossf-cve-benchmark/CVE-2017-16114) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16114.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16114.svg)

## CVE-2017-16098
 charset 1.0.0 and below are vulnerable to regular expression denial of service. Input of around 50k characters is required for a slow down of around 2 seconds. Unless node was compiled using the -DHTTP_MAX_HEADER_SIZE= option the default header max length is 80kb, so the impact of the ReDoS is relatively low.



- [https://github.com/ossf-cve-benchmark/CVE-2017-16098](https://github.com/ossf-cve-benchmark/CVE-2017-16098) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16098.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16098.svg)

## CVE-2017-16088
 The safe-eval module describes itself as a safer version of eval. By accessing the object constructors, un-sanitized user input can access the entire standard library and effectively break out of the sandbox.



- [https://github.com/Flyy-yu/CVE-2017-16088](https://github.com/Flyy-yu/CVE-2017-16088) :  ![starts](https://img.shields.io/github/stars/Flyy-yu/CVE-2017-16088.svg) ![forks](https://img.shields.io/github/forks/Flyy-yu/CVE-2017-16088.svg)

## CVE-2017-16087
 ** RESERVED ** This candidate has been reserved by an organization or individual that will use it when announcing a new security problem.  When the candidate has been publicized, the details for this candidate will be provided.



- [https://github.com/ossf-cve-benchmark/CVE-2017-16087](https://github.com/ossf-cve-benchmark/CVE-2017-16087) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16087.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16087.svg)

## CVE-2017-16084
 list-n-stream is a server for static files to list and stream local videos. list-n-stream v0.0.10 or lower is vulnerable to a directory traversal issue, giving an attacker access to the filesystem by placing "../" in the url.



- [https://github.com/ossf-cve-benchmark/CVE-2017-16084](https://github.com/ossf-cve-benchmark/CVE-2017-16084) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16084.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16084.svg)

## CVE-2017-16034
 ** RESERVED ** This candidate has been reserved by an organization or individual that will use it when announcing a new security problem.  When the candidate has been publicized, the details for this candidate will be provided.



- [https://github.com/ossf-cve-benchmark/CVE-2017-16034](https://github.com/ossf-cve-benchmark/CVE-2017-16034) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16034.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16034.svg)

## CVE-2017-16031
 Socket.io is a realtime application framework that provides communication via websockets. Because socket.io 0.9.6 and earlier depends on `Math.random()` to create socket IDs, the IDs are predictable. An attacker is able to guess the socket ID and gain access to socket.io servers, potentially obtaining sensitive information.



- [https://github.com/ossf-cve-benchmark/CVE-2017-16031](https://github.com/ossf-cve-benchmark/CVE-2017-16031) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16031.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16031.svg)

## CVE-2017-16023
 Decamelize is used to convert a dash/dot/underscore/space separated string to camelCase. Decamelize 1.1.0 through 1.1.1 uses regular expressions to evaluate a string and takes unescaped separator values, which can be used to create a denial of service attack.



- [https://github.com/CQ-Tools/CVE-2017-16023-fixed](https://github.com/CQ-Tools/CVE-2017-16023-fixed) :  ![starts](https://img.shields.io/github/stars/CQ-Tools/CVE-2017-16023-fixed.svg) ![forks](https://img.shields.io/github/forks/CQ-Tools/CVE-2017-16023-fixed.svg)

- [https://github.com/CQ-Tools/CVE-2017-16023-unfixed](https://github.com/CQ-Tools/CVE-2017-16023-unfixed) :  ![starts](https://img.shields.io/github/stars/CQ-Tools/CVE-2017-16023-unfixed.svg) ![forks](https://img.shields.io/github/forks/CQ-Tools/CVE-2017-16023-unfixed.svg)

- [https://github.com/ossf-cve-benchmark/CVE-2017-16023](https://github.com/ossf-cve-benchmark/CVE-2017-16023) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-16023.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-16023.svg)

## CVE-2017-15944
 Palo Alto Networks PAN-OS before 6.1.19, 7.0.x before 7.0.19, 7.1.x before 7.1.14, and 8.0.x before 8.0.6 allows remote attackers to execute arbitrary code via vectors involving the management interface.



- [https://github.com/surajraghuvanshi/PaloAltoRceDetectionAndExploit](https://github.com/surajraghuvanshi/PaloAltoRceDetectionAndExploit) :  ![starts](https://img.shields.io/github/stars/surajraghuvanshi/PaloAltoRceDetectionAndExploit.svg) ![forks](https://img.shields.io/github/forks/surajraghuvanshi/PaloAltoRceDetectionAndExploit.svg)

- [https://github.com/xxnbyy/CVE-2017-15944-POC](https://github.com/xxnbyy/CVE-2017-15944-POC) :  ![starts](https://img.shields.io/github/stars/xxnbyy/CVE-2017-15944-POC.svg) ![forks](https://img.shields.io/github/forks/xxnbyy/CVE-2017-15944-POC.svg)

- [https://github.com/P4x1s/PaloAlto_EXP](https://github.com/P4x1s/PaloAlto_EXP) :  ![starts](https://img.shields.io/github/stars/P4x1s/PaloAlto_EXP.svg) ![forks](https://img.shields.io/github/forks/P4x1s/PaloAlto_EXP.svg)

- [https://github.com/yukar1z0e/CVE-2017-15944](https://github.com/yukar1z0e/CVE-2017-15944) :  ![starts](https://img.shields.io/github/stars/yukar1z0e/CVE-2017-15944.svg) ![forks](https://img.shields.io/github/forks/yukar1z0e/CVE-2017-15944.svg)

## CVE-2017-15689
 ** RESERVED ** This candidate has been reserved by an organization or individual that will use it when announcing a new security problem.  When the candidate has been publicized, the details for this candidate will be provided.



- [https://github.com/hidog123/Codiad-CVE-2018-14009](https://github.com/hidog123/Codiad-CVE-2018-14009) :  ![starts](https://img.shields.io/github/stars/hidog123/Codiad-CVE-2018-14009.svg) ![forks](https://img.shields.io/github/forks/hidog123/Codiad-CVE-2018-14009.svg)

## CVE-2017-15303
 In CPUID CPU-Z before 1.43, there is an arbitrary memory write that results directly in elevation of privileges, because any program running on the local machine (while CPU-Z is running) can issue an ioctl 0x9C402430 call to the kernel-mode driver (e.g., cpuz141_x64.sys for version 1.41).



- [https://github.com/hfiref0x/Stryker](https://github.com/hfiref0x/Stryker) :  ![starts](https://img.shields.io/github/stars/hfiref0x/Stryker.svg) ![forks](https://img.shields.io/github/forks/hfiref0x/Stryker.svg)

## CVE-2017-14948
 Certain D-Link products are affected by: Buffer Overflow. This affects DIR-880L 1.08B04 and DIR-895 L/R 1.13b03. The impact is: execute arbitrary code (remote). The component is: htdocs/fileaccess.cgi. The attack vector is: A crafted HTTP request handled by fileacces.cgi could allow an attacker to mount a ROP attack: if the HTTP header field CONTENT_TYPE starts with ''boundary=' followed by more than 256 characters, a buffer overflow would be triggered, potentially causing code execution.



- [https://github.com/badnack/d_link_880_bug](https://github.com/badnack/d_link_880_bug) :  ![starts](https://img.shields.io/github/stars/badnack/d_link_880_bug.svg) ![forks](https://img.shields.io/github/forks/badnack/d_link_880_bug.svg)

## CVE-2017-14719
 Before version 4.8.2, WordPress was vulnerable to a directory traversal attack during unzip operations in the ZipArchive and PclZip components.



- [https://github.com/PalmTreeForest/CodePath_Week_7-8](https://github.com/PalmTreeForest/CodePath_Week_7-8) :  ![starts](https://img.shields.io/github/stars/PalmTreeForest/CodePath_Week_7-8.svg) ![forks](https://img.shields.io/github/forks/PalmTreeForest/CodePath_Week_7-8.svg)

## CVE-2017-14494
 dnsmasq before 2.78, when configured as a relay, allows remote attackers to obtain sensitive memory information via vectors involving handling DHCPv6 forwarded requests.



- [https://github.com/raw-packet/raw-packet](https://github.com/raw-packet/raw-packet) :  ![starts](https://img.shields.io/github/stars/raw-packet/raw-packet.svg) ![forks](https://img.shields.io/github/forks/raw-packet/raw-packet.svg)

## CVE-2017-14322
 The function in charge to check whether the user is already logged in init.php in Interspire Email Marketer (IEM) prior to 6.1.6 allows remote attackers to bypass authentication and obtain administrative access by using the IEM_CookieLogin cookie with a specially crafted value.



- [https://github.com/joesmithjaffa/CVE-2017-14322](https://github.com/joesmithjaffa/CVE-2017-14322) :  ![starts](https://img.shields.io/github/stars/joesmithjaffa/CVE-2017-14322.svg) ![forks](https://img.shields.io/github/forks/joesmithjaffa/CVE-2017-14322.svg)

## CVE-2017-13672
 QEMU (aka Quick Emulator), when built with the VGA display emulator support, allows local guest OS privileged users to cause a denial of service (out-of-bounds read and QEMU process crash) via vectors involving display update.



- [https://github.com/DavidBuchanan314/CVE-2017-13672](https://github.com/DavidBuchanan314/CVE-2017-13672) :  ![starts](https://img.shields.io/github/stars/DavidBuchanan314/CVE-2017-13672.svg) ![forks](https://img.shields.io/github/forks/DavidBuchanan314/CVE-2017-13672.svg)

## CVE-2017-13286
 In writeToParcel and readFromParcel of OutputConfiguration.java, there is a permission bypass due to mismatched serialization. This could lead to a local escalation of privilege where the user can start an activity with system privileges, with no additional execution privileges needed. User interaction is not needed for exploitation. Product: Android. Versions: 8.0, 8.1. Android ID: A-69683251.



- [https://github.com/UmVfX1BvaW50/CVE-2017-13286](https://github.com/UmVfX1BvaW50/CVE-2017-13286) :  ![starts](https://img.shields.io/github/stars/UmVfX1BvaW50/CVE-2017-13286.svg) ![forks](https://img.shields.io/github/forks/UmVfX1BvaW50/CVE-2017-13286.svg)

## CVE-2017-12792
 Multiple cross-site request forgery (CSRF) vulnerabilities in NexusPHP 1.5 allow remote attackers to hijack the authentication of administrators for requests that conduct cross-site scripting (XSS) attacks via the (1) linkname, (2) url, or (3) title parameter in an add action to linksmanage.php.



- [https://github.com/ZZS2017/cve-2017-12792](https://github.com/ZZS2017/cve-2017-12792) :  ![starts](https://img.shields.io/github/stars/ZZS2017/cve-2017-12792.svg) ![forks](https://img.shields.io/github/forks/ZZS2017/cve-2017-12792.svg)

## CVE-2017-12637
 Directory traversal vulnerability in scheduler/ui/js/ffffffffbca41eb4/UIUtilJavaScriptJS in SAP NetWeaver Application Server Java 7.5 allows remote attackers to read arbitrary files via a .. (dot dot) in the query string, as exploited in the wild in August 2017, aka SAP Security Note 2486657.



- [https://github.com/abrewer251/CVE-2017-12637_SAP-NetWeaver-URL-Traversal](https://github.com/abrewer251/CVE-2017-12637_SAP-NetWeaver-URL-Traversal) :  ![starts](https://img.shields.io/github/stars/abrewer251/CVE-2017-12637_SAP-NetWeaver-URL-Traversal.svg) ![forks](https://img.shields.io/github/forks/abrewer251/CVE-2017-12637_SAP-NetWeaver-URL-Traversal.svg)

## CVE-2017-12426
 GitLab Community Edition (CE) and Enterprise Edition (EE) before 8.17.8, 9.0.x before 9.0.13, 9.1.x before 9.1.10, 9.2.x before 9.2.10, 9.3.x before 9.3.10, and 9.4.x before 9.4.4 might allow remote attackers to execute arbitrary code via a crafted SSH URL in a project import.



- [https://github.com/sm-paul-schuette/CVE-2017-12426](https://github.com/sm-paul-schuette/CVE-2017-12426) :  ![starts](https://img.shields.io/github/stars/sm-paul-schuette/CVE-2017-12426.svg) ![forks](https://img.shields.io/github/forks/sm-paul-schuette/CVE-2017-12426.svg)

## CVE-2017-11826
 Microsoft Office 2010, SharePoint Enterprise Server 2010, SharePoint Server 2010, Web Applications, Office Web Apps Server 2010 and 2013, Word Viewer, Word 2007, 2010, 2013 and 2016, Word Automation Services, and Office Online Server allow remote code execution when the software fails to properly handle objects in memory.



- [https://github.com/thatskriptkid/CVE-2017-11826](https://github.com/thatskriptkid/CVE-2017-11826) :  ![starts](https://img.shields.io/github/stars/thatskriptkid/CVE-2017-11826.svg) ![forks](https://img.shields.io/github/forks/thatskriptkid/CVE-2017-11826.svg)

- [https://github.com/9aylas/DDE-MS_WORD-Exploit_Detector](https://github.com/9aylas/DDE-MS_WORD-Exploit_Detector) :  ![starts](https://img.shields.io/github/stars/9aylas/DDE-MS_WORD-Exploit_Detector.svg) ![forks](https://img.shields.io/github/forks/9aylas/DDE-MS_WORD-Exploit_Detector.svg)

## CVE-2017-11611
 Wolf CMS 0.8.3.1 allows Cross-Site Scripting (XSS) attacks. The vulnerability exists due to insufficient sanitization of the file name in a "create-file-popup" action, and the directory name in a "create-directory-popup" action, in the HTTP POST method to the "/plugin/file_manager/" script (aka an /admin/plugin/file_manager/browse// URI).



- [https://github.com/faizzaidi/Wolfcms-v0.8.3.1-xss-POC-by-Provensec-llc](https://github.com/faizzaidi/Wolfcms-v0.8.3.1-xss-POC-by-Provensec-llc) :  ![starts](https://img.shields.io/github/stars/faizzaidi/Wolfcms-v0.8.3.1-xss-POC-by-Provensec-llc.svg) ![forks](https://img.shields.io/github/forks/faizzaidi/Wolfcms-v0.8.3.1-xss-POC-by-Provensec-llc.svg)

## CVE-2017-11610
 The XML-RPC server in supervisor before 3.0.1, 3.1.x before 3.1.4, 3.2.x before 3.2.4, and 3.3.x before 3.3.3 allows remote authenticated users to execute arbitrary commands via a crafted XML-RPC request, related to nested supervisord namespace lookups.



- [https://github.com/yaunsky/CVE-2017-11610](https://github.com/yaunsky/CVE-2017-11610) :  ![starts](https://img.shields.io/github/stars/yaunsky/CVE-2017-11610.svg) ![forks](https://img.shields.io/github/forks/yaunsky/CVE-2017-11610.svg)

- [https://github.com/ivanitlearning/CVE-2017-11610](https://github.com/ivanitlearning/CVE-2017-11610) :  ![starts](https://img.shields.io/github/stars/ivanitlearning/CVE-2017-11610.svg) ![forks](https://img.shields.io/github/forks/ivanitlearning/CVE-2017-11610.svg)

## CVE-2017-11503
 PHPMailer 5.2.23 has XSS in the "From Email Address" and "To Email Address" fields of code_generator.php.



- [https://github.com/wizardafric/download](https://github.com/wizardafric/download) :  ![starts](https://img.shields.io/github/stars/wizardafric/download.svg) ![forks](https://img.shields.io/github/forks/wizardafric/download.svg)

## CVE-2017-11176
 The mq_notify function in the Linux kernel through 4.11.9 does not set the sock pointer to NULL upon entry into the retry logic. During a user-space close of a Netlink socket, it allows attackers to cause a denial of service (use-after-free) or possibly have unspecified other impact.



- [https://github.com/lexfo/cve-2017-11176](https://github.com/lexfo/cve-2017-11176) :  ![starts](https://img.shields.io/github/stars/lexfo/cve-2017-11176.svg) ![forks](https://img.shields.io/github/forks/lexfo/cve-2017-11176.svg)

- [https://github.com/c3r34lk1ll3r/CVE-2017-11176](https://github.com/c3r34lk1ll3r/CVE-2017-11176) :  ![starts](https://img.shields.io/github/stars/c3r34lk1ll3r/CVE-2017-11176.svg) ![forks](https://img.shields.io/github/forks/c3r34lk1ll3r/CVE-2017-11176.svg)

- [https://github.com/Sama-Ayman-Mokhtar/CVE-2017-11176](https://github.com/Sama-Ayman-Mokhtar/CVE-2017-11176) :  ![starts](https://img.shields.io/github/stars/Sama-Ayman-Mokhtar/CVE-2017-11176.svg) ![forks](https://img.shields.io/github/forks/Sama-Ayman-Mokhtar/CVE-2017-11176.svg)

- [https://github.com/Cyb3rCr0wCC/cve-2017-11176](https://github.com/Cyb3rCr0wCC/cve-2017-11176) :  ![starts](https://img.shields.io/github/stars/Cyb3rCr0wCC/cve-2017-11176.svg) ![forks](https://img.shields.io/github/forks/Cyb3rCr0wCC/cve-2017-11176.svg)

- [https://github.com/Yanoro/CVE-2017-11176](https://github.com/Yanoro/CVE-2017-11176) :  ![starts](https://img.shields.io/github/stars/Yanoro/CVE-2017-11176.svg) ![forks](https://img.shields.io/github/forks/Yanoro/CVE-2017-11176.svg)

- [https://github.com/leonardo1101/cve-2017-11176](https://github.com/leonardo1101/cve-2017-11176) :  ![starts](https://img.shields.io/github/stars/leonardo1101/cve-2017-11176.svg) ![forks](https://img.shields.io/github/forks/leonardo1101/cve-2017-11176.svg)

- [https://github.com/DoubleMice/cve-2017-11176](https://github.com/DoubleMice/cve-2017-11176) :  ![starts](https://img.shields.io/github/stars/DoubleMice/cve-2017-11176.svg) ![forks](https://img.shields.io/github/forks/DoubleMice/cve-2017-11176.svg)

## CVE-2017-10910
 MQTT.js 2.x.x prior to 2.15.0 issue in handling PUBLISH tickets may lead to an attacker causing a denial-of-service condition.



- [https://github.com/ossf-cve-benchmark/CVE-2017-10910](https://github.com/ossf-cve-benchmark/CVE-2017-10910) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-10910.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-10910.svg)

## CVE-2017-10797
 ** RESERVED ** This candidate has been reserved by an organization or individual that will use it when announcing a new security problem.  When the candidate has been publicized, the details for this candidate will be provided.



- [https://github.com/n4xh4ck5/CVE-2017-10797](https://github.com/n4xh4ck5/CVE-2017-10797) :  ![starts](https://img.shields.io/github/stars/n4xh4ck5/CVE-2017-10797.svg) ![forks](https://img.shields.io/github/forks/n4xh4ck5/CVE-2017-10797.svg)

## CVE-2017-10416
 Vulnerability in the Oracle Advanced Outbound Telephony component of Oracle E-Business Suite (subcomponent: Setup and Configuration). Supported versions that are affected are 12.2.3, 12.2.4, 12.2.5, 12.2.6 and 12.2.7. Easily exploitable vulnerability allows unauthenticated attacker with network access via HTTP to compromise Oracle Advanced Outbound Telephony. Successful attacks require human interaction from a person other than the attacker and while the vulnerability is in Oracle Advanced Outbound Telephony, attacks may significantly impact additional products. Successful attacks of this vulnerability can result in unauthorized access to critical data or complete access to all Oracle Advanced Outbound Telephony accessible data as well as unauthorized update, insert or delete access to some of Oracle Advanced Outbound Telephony accessible data. CVSS 3.0 Base Score 8.2 (Confidentiality and Integrity impacts). CVSS Vector: (CVSS:3.0/AV:N/AC:L/PR:N/UI:R/S:C/C:H/I:L/A:N).



- [https://github.com/vah13/OracleCVE](https://github.com/vah13/OracleCVE) :  ![starts](https://img.shields.io/github/stars/vah13/OracleCVE.svg) ![forks](https://img.shields.io/github/forks/vah13/OracleCVE.svg)

## CVE-2017-9947
 A vulnerability has been identified in Siemens APOGEE PXC and TALON TC BACnet Automation Controllers in all versions V3.5. A directory traversal vulnerability could allow a remote attacker with network access to the integrated web server (80/tcp and 443/tcp) to obtain information on the structure of the file system of the affected devices.



- [https://github.com/RoseSecurity/APOLOGEE](https://github.com/RoseSecurity/APOLOGEE) :  ![starts](https://img.shields.io/github/stars/RoseSecurity/APOLOGEE.svg) ![forks](https://img.shields.io/github/forks/RoseSecurity/APOLOGEE.svg)

## CVE-2017-9830
 Remote Code Execution is possible in Code42 CrashPlan 5.4.x via the org.apache.commons.ssl.rmi.DateRMI Java class, because (upon instantiation) it creates an RMI server that listens on a TCP port and deserializes objects sent by TCP clients.



- [https://github.com/securifera/CVE-2017-9830](https://github.com/securifera/CVE-2017-9830) :  ![starts](https://img.shields.io/github/stars/securifera/CVE-2017-9830.svg) ![forks](https://img.shields.io/github/forks/securifera/CVE-2017-9830.svg)

## CVE-2017-9779
 OCaml compiler allows attackers to have unspecified impact via unknown vectors, a similar issue to CVE-2017-9772 "but with much less impact."



- [https://github.com/homjxi0e/CVE-2017-9779](https://github.com/homjxi0e/CVE-2017-9779) :  ![starts](https://img.shields.io/github/stars/homjxi0e/CVE-2017-9779.svg) ![forks](https://img.shields.io/github/forks/homjxi0e/CVE-2017-9779.svg)

## CVE-2017-9609
 Cross-site scripting (XSS) vulnerability in Blackcat CMS 1.2 allows remote authenticated users to inject arbitrary web script or HTML via the map_language parameter to backend/pages/lang_settings.php.



- [https://github.com/faizzaidi/Blackcat-cms-v1.2-xss-POC-by-Provensec-llc](https://github.com/faizzaidi/Blackcat-cms-v1.2-xss-POC-by-Provensec-llc) :  ![starts](https://img.shields.io/github/stars/faizzaidi/Blackcat-cms-v1.2-xss-POC-by-Provensec-llc.svg) ![forks](https://img.shields.io/github/forks/faizzaidi/Blackcat-cms-v1.2-xss-POC-by-Provensec-llc.svg)

## CVE-2017-9506
 The IconUriServlet of the Atlassian OAuth Plugin from version 1.3.0 before version 1.9.12 and from version 2.0.0 before version 2.0.4 allows remote attackers to access the content of internal network resources and/or perform an XSS attack via Server Side Request Forgery (SSRF).



- [https://github.com/random-robbie/Jira-Scan](https://github.com/random-robbie/Jira-Scan) :  ![starts](https://img.shields.io/github/stars/random-robbie/Jira-Scan.svg) ![forks](https://img.shields.io/github/forks/random-robbie/Jira-Scan.svg)

- [https://github.com/labsbots/CVE-2017-9506](https://github.com/labsbots/CVE-2017-9506) :  ![starts](https://img.shields.io/github/stars/labsbots/CVE-2017-9506.svg) ![forks](https://img.shields.io/github/forks/labsbots/CVE-2017-9506.svg)

- [https://github.com/pwn1sher/jira-ssrf](https://github.com/pwn1sher/jira-ssrf) :  ![starts](https://img.shields.io/github/stars/pwn1sher/jira-ssrf.svg) ![forks](https://img.shields.io/github/forks/pwn1sher/jira-ssrf.svg)

## CVE-2017-9101
 import.php (aka the Phonebook import feature) in PlaySMS 1.4 allows remote code execution via vectors involving the User-Agent HTTP header and PHP code in the name of a file.



- [https://github.com/jasperla/CVE-2017-9101](https://github.com/jasperla/CVE-2017-9101) :  ![starts](https://img.shields.io/github/stars/jasperla/CVE-2017-9101.svg) ![forks](https://img.shields.io/github/forks/jasperla/CVE-2017-9101.svg)

## CVE-2017-8809
 api.php in MediaWiki before 1.27.4, 1.28.x before 1.28.3, and 1.29.x before 1.29.2 has a Reflected File Download vulnerability.



- [https://github.com/motikan2010/CVE-2017-8809_MediaWiki_RFD](https://github.com/motikan2010/CVE-2017-8809_MediaWiki_RFD) :  ![starts](https://img.shields.io/github/stars/motikan2010/CVE-2017-8809_MediaWiki_RFD.svg) ![forks](https://img.shields.io/github/forks/motikan2010/CVE-2017-8809_MediaWiki_RFD.svg)

## CVE-2017-8802
 Cross-site scripting (XSS) vulnerability in Zimbra Collaboration Suite (aka ZCS) before 8.8.0 Beta2 might allow remote attackers to inject arbitrary web script or HTML via vectors related to the "Show Snippet" functionality.



- [https://github.com/ozzi-/Zimbra-CVE-2017-8802-Hotifx](https://github.com/ozzi-/Zimbra-CVE-2017-8802-Hotifx) :  ![starts](https://img.shields.io/github/stars/ozzi-/Zimbra-CVE-2017-8802-Hotifx.svg) ![forks](https://img.shields.io/github/forks/ozzi-/Zimbra-CVE-2017-8802-Hotifx.svg)

## CVE-2017-8759
 Microsoft .NET Framework 2.0, 3.5, 3.5.1, 4.5.2, 4.6, 4.6.1, 4.6.2 and 4.7 allow an attacker to execute code remotely via a malicious document or application, aka ".NET Framework Remote Code Execution Vulnerability."



- [https://github.com/bhdresh/CVE-2017-8759](https://github.com/bhdresh/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/bhdresh/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/bhdresh/CVE-2017-8759.svg)

- [https://github.com/Voulnet/CVE-2017-8759-Exploit-sample](https://github.com/Voulnet/CVE-2017-8759-Exploit-sample) :  ![starts](https://img.shields.io/github/stars/Voulnet/CVE-2017-8759-Exploit-sample.svg) ![forks](https://img.shields.io/github/forks/Voulnet/CVE-2017-8759-Exploit-sample.svg)

- [https://github.com/vysecurity/CVE-2017-8759](https://github.com/vysecurity/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/vysecurity/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/vysecurity/CVE-2017-8759.svg)

- [https://github.com/nccgroup/CVE-2017-8759](https://github.com/nccgroup/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/nccgroup/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/nccgroup/CVE-2017-8759.svg)

- [https://github.com/JonasUliana/CVE-2017-8759](https://github.com/JonasUliana/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/JonasUliana/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/JonasUliana/CVE-2017-8759.svg)

- [https://github.com/jacobsoo/RTF-Cleaner](https://github.com/jacobsoo/RTF-Cleaner) :  ![starts](https://img.shields.io/github/stars/jacobsoo/RTF-Cleaner.svg) ![forks](https://img.shields.io/github/forks/jacobsoo/RTF-Cleaner.svg)

- [https://github.com/ashr/CVE-2017-8759-exploits](https://github.com/ashr/CVE-2017-8759-exploits) :  ![starts](https://img.shields.io/github/stars/ashr/CVE-2017-8759-exploits.svg) ![forks](https://img.shields.io/github/forks/ashr/CVE-2017-8759-exploits.svg)

- [https://github.com/homjxi0e/CVE-2017-8759_-SOAP_WSDL](https://github.com/homjxi0e/CVE-2017-8759_-SOAP_WSDL) :  ![starts](https://img.shields.io/github/stars/homjxi0e/CVE-2017-8759_-SOAP_WSDL.svg) ![forks](https://img.shields.io/github/forks/homjxi0e/CVE-2017-8759_-SOAP_WSDL.svg)

- [https://github.com/BasuCert/CVE-2017-8759](https://github.com/BasuCert/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/BasuCert/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/BasuCert/CVE-2017-8759.svg)

- [https://github.com/sythass/CVE-2017-8759](https://github.com/sythass/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/sythass/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/sythass/CVE-2017-8759.svg)

- [https://github.com/ChaitanyaHaritash/CVE-2017-8759](https://github.com/ChaitanyaHaritash/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/ChaitanyaHaritash/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/ChaitanyaHaritash/CVE-2017-8759.svg)

- [https://github.com/zhengkook/CVE-2017-8759](https://github.com/zhengkook/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/zhengkook/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/zhengkook/CVE-2017-8759.svg)

- [https://github.com/adeljck/CVE-2017-8759](https://github.com/adeljck/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/adeljck/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/adeljck/CVE-2017-8759.svg)

- [https://github.com/l0n3rs/CVE-2017-8759](https://github.com/l0n3rs/CVE-2017-8759) :  ![starts](https://img.shields.io/github/stars/l0n3rs/CVE-2017-8759.svg) ![forks](https://img.shields.io/github/forks/l0n3rs/CVE-2017-8759.svg)

- [https://github.com/Winter3un/cve_2017_8759](https://github.com/Winter3un/cve_2017_8759) :  ![starts](https://img.shields.io/github/stars/Winter3un/cve_2017_8759.svg) ![forks](https://img.shields.io/github/forks/Winter3un/cve_2017_8759.svg)

- [https://github.com/smashinu/CVE-2017-8759Expoit](https://github.com/smashinu/CVE-2017-8759Expoit) :  ![starts](https://img.shields.io/github/stars/smashinu/CVE-2017-8759Expoit.svg) ![forks](https://img.shields.io/github/forks/smashinu/CVE-2017-8759Expoit.svg)

- [https://github.com/tahisaad6/CVE-2017-8759-Exploit-sample2](https://github.com/tahisaad6/CVE-2017-8759-Exploit-sample2) :  ![starts](https://img.shields.io/github/stars/tahisaad6/CVE-2017-8759-Exploit-sample2.svg) ![forks](https://img.shields.io/github/forks/tahisaad6/CVE-2017-8759-Exploit-sample2.svg)

- [https://github.com/GayashanM/OHTS](https://github.com/GayashanM/OHTS) :  ![starts](https://img.shields.io/github/stars/GayashanM/OHTS.svg) ![forks](https://img.shields.io/github/forks/GayashanM/OHTS.svg)

- [https://github.com/varunsaru/SNP](https://github.com/varunsaru/SNP) :  ![starts](https://img.shields.io/github/stars/varunsaru/SNP.svg) ![forks](https://img.shields.io/github/forks/varunsaru/SNP.svg)

- [https://github.com/chefphenix25/vuln-rabilit-windows7](https://github.com/chefphenix25/vuln-rabilit-windows7) :  ![starts](https://img.shields.io/github/stars/chefphenix25/vuln-rabilit-windows7.svg) ![forks](https://img.shields.io/github/forks/chefphenix25/vuln-rabilit-windows7.svg)

## CVE-2017-8543
 Microsoft Windows XP SP3, Windows XP x64 XP2, Windows Server 2003 SP2, Windows Vista, Windows 7 SP1, Windows Server 2008 SP2 and R2 SP1, Windows 8, Windows 8.1 and Windows RT 8.1, Windows Server 2012 and R2, Windows 10 Gold, 1511, 1607, and 1703, and Windows Server 2016 allow an attacker to take control of the affected system when Windows Search fails to handle objects in memory, aka "Windows Search Remote Code Execution Vulnerability".



- [https://github.com/americanhanko/windows-security-cve-2017-8543](https://github.com/americanhanko/windows-security-cve-2017-8543) :  ![starts](https://img.shields.io/github/stars/americanhanko/windows-security-cve-2017-8543.svg) ![forks](https://img.shields.io/github/forks/americanhanko/windows-security-cve-2017-8543.svg)

## CVE-2017-8382
 admidio 3.2.8 has CSRF in adm_program/modules/members/members_function.php with an impact of deleting arbitrary user accounts.



- [https://github.com/faizzaidi/Admidio-3.2.8-CSRF-POC-by-Provensec-llc](https://github.com/faizzaidi/Admidio-3.2.8-CSRF-POC-by-Provensec-llc) :  ![starts](https://img.shields.io/github/stars/faizzaidi/Admidio-3.2.8-CSRF-POC-by-Provensec-llc.svg) ![forks](https://img.shields.io/github/forks/faizzaidi/Admidio-3.2.8-CSRF-POC-by-Provensec-llc.svg)

## CVE-2017-8367
 Buffer overflow in Ether Software Easy MOV Converter 1.4.24, Easy DVD Creator, Easy MPEG/AVI/DIVX/WMV/RM to DVD, Easy Avi/Divx/Xvid to DVD Burner, Easy MPEG to DVD Burner, Easy WMV/ASF/ASX to DVD Burner, Easy RM RMVB to DVD Burner, Easy CD DVD Copy, MP3/AVI/MPEG/WMV/RM to Audio CD Burner, MP3/WAV/OGG/WMA/AC3 to CD Burner, MP3 WAV to CD Burner, My Video Converter, Easy AVI DivX Converter, Easy Video to iPod Converter, Easy Video to PSP Converter, Easy Video to 3GP Converter, Easy Video to MP4 Converter, and Easy Video to iPod/MP4/PSP/3GP Converter allows local attackers to cause a denial of service (SEH overwrite) or possibly have unspecified other impact via a long username.



- [https://github.com/rnnsz/CVE-2017-8367](https://github.com/rnnsz/CVE-2017-8367) :  ![starts](https://img.shields.io/github/stars/rnnsz/CVE-2017-8367.svg) ![forks](https://img.shields.io/github/forks/rnnsz/CVE-2017-8367.svg)

## CVE-2017-8295
 WordPress through 4.7.4 relies on the Host HTTP header for a password-reset e-mail message, which makes it easier for remote attackers to reset arbitrary passwords by making a crafted wp-login.php?action=lostpassword request and then arranging for this message to bounce or be resent, leading to transmission of the reset key to a mailbox on an attacker-controlled SMTP server. This is related to problematic use of the SERVER_NAME variable in wp-includes/pluggable.php in conjunction with the PHP mail function. Exploitation is not achievable in all cases because it requires at least one of the following: (1) the attacker can prevent the victim from receiving any e-mail messages for an extended period of time (such as 5 days), (2) the victim's e-mail system sends an autoresponse containing the original message, or (3) the victim manually composes a reply containing the original message.



- [https://github.com/cyberheartmi9/CVE-2017-8295](https://github.com/cyberheartmi9/CVE-2017-8295) :  ![starts](https://img.shields.io/github/stars/cyberheartmi9/CVE-2017-8295.svg) ![forks](https://img.shields.io/github/forks/cyberheartmi9/CVE-2017-8295.svg)

- [https://github.com/alash3al/wp-allowed-hosts](https://github.com/alash3al/wp-allowed-hosts) :  ![starts](https://img.shields.io/github/stars/alash3al/wp-allowed-hosts.svg) ![forks](https://img.shields.io/github/forks/alash3al/wp-allowed-hosts.svg)

- [https://github.com/homjxi0e/CVE-2017-8295-WordPress-4.7.4---Unauthorized-Password-Reset](https://github.com/homjxi0e/CVE-2017-8295-WordPress-4.7.4---Unauthorized-Password-Reset) :  ![starts](https://img.shields.io/github/stars/homjxi0e/CVE-2017-8295-WordPress-4.7.4---Unauthorized-Password-Reset.svg) ![forks](https://img.shields.io/github/forks/homjxi0e/CVE-2017-8295-WordPress-4.7.4---Unauthorized-Password-Reset.svg)

## CVE-2017-8056
 WatchGuard Fireware v11.12.1 and earlier mishandles requests referring to an XML External Entity (XXE), in the XML-RPC agent. This causes the Firebox wgagent process to crash. This process crash ends all authenticated sessions to the Firebox, including management connections, and prevents new authenticated sessions until the process has recovered. The Firebox may also experience an overall degradation in performance while the wgagent process recovers. An attacker could continuously send XML-RPC requests that contain references to external entities to perform a limited Denial of Service (DoS) attack against an affected Firebox.



- [https://github.com/itzexploit/CVE-2017-8056](https://github.com/itzexploit/CVE-2017-8056) :  ![starts](https://img.shields.io/github/stars/itzexploit/CVE-2017-8056.svg) ![forks](https://img.shields.io/github/forks/itzexploit/CVE-2017-8056.svg)

## CVE-2017-8046
 Malicious PATCH requests submitted to servers using Spring Data REST versions prior to 2.6.9 (Ingalls SR9), versions prior to 3.0.1 (Kay SR1) and Spring Boot versions prior to 1.5.9, 2.0 M6 can use specially crafted JSON data to run arbitrary Java code.



- [https://github.com/m3ssap0/spring-break_cve-2017-8046](https://github.com/m3ssap0/spring-break_cve-2017-8046) :  ![starts](https://img.shields.io/github/stars/m3ssap0/spring-break_cve-2017-8046.svg) ![forks](https://img.shields.io/github/forks/m3ssap0/spring-break_cve-2017-8046.svg)

- [https://github.com/m3ssap0/SpringBreakVulnerableApp](https://github.com/m3ssap0/SpringBreakVulnerableApp) :  ![starts](https://img.shields.io/github/stars/m3ssap0/SpringBreakVulnerableApp.svg) ![forks](https://img.shields.io/github/forks/m3ssap0/SpringBreakVulnerableApp.svg)

- [https://github.com/Soontao/CVE-2017-8046-DEMO](https://github.com/Soontao/CVE-2017-8046-DEMO) :  ![starts](https://img.shields.io/github/stars/Soontao/CVE-2017-8046-DEMO.svg) ![forks](https://img.shields.io/github/forks/Soontao/CVE-2017-8046-DEMO.svg)

- [https://github.com/cved-sources/cve-2017-8046](https://github.com/cved-sources/cve-2017-8046) :  ![starts](https://img.shields.io/github/stars/cved-sources/cve-2017-8046.svg) ![forks](https://img.shields.io/github/forks/cved-sources/cve-2017-8046.svg)

- [https://github.com/FixYourFace/SpringBreakPoC](https://github.com/FixYourFace/SpringBreakPoC) :  ![starts](https://img.shields.io/github/stars/FixYourFace/SpringBreakPoC.svg) ![forks](https://img.shields.io/github/forks/FixYourFace/SpringBreakPoC.svg)

- [https://github.com/jkutner/spring-break-cve-2017-8046](https://github.com/jkutner/spring-break-cve-2017-8046) :  ![starts](https://img.shields.io/github/stars/jkutner/spring-break-cve-2017-8046.svg) ![forks](https://img.shields.io/github/forks/jkutner/spring-break-cve-2017-8046.svg)

- [https://github.com/sj/spring-data-rest-CVE-2017-8046](https://github.com/sj/spring-data-rest-CVE-2017-8046) :  ![starts](https://img.shields.io/github/stars/sj/spring-data-rest-CVE-2017-8046.svg) ![forks](https://img.shields.io/github/forks/sj/spring-data-rest-CVE-2017-8046.svg)

- [https://github.com/bkhablenko/CVE-2017-8046](https://github.com/bkhablenko/CVE-2017-8046) :  ![starts](https://img.shields.io/github/stars/bkhablenko/CVE-2017-8046.svg) ![forks](https://img.shields.io/github/forks/bkhablenko/CVE-2017-8046.svg)

- [https://github.com/guanjivip/CVE-2017-8046](https://github.com/guanjivip/CVE-2017-8046) :  ![starts](https://img.shields.io/github/stars/guanjivip/CVE-2017-8046.svg) ![forks](https://img.shields.io/github/forks/guanjivip/CVE-2017-8046.svg)

- [https://github.com/jsotiro/VulnerableSpringDataRest](https://github.com/jsotiro/VulnerableSpringDataRest) :  ![starts](https://img.shields.io/github/stars/jsotiro/VulnerableSpringDataRest.svg) ![forks](https://img.shields.io/github/forks/jsotiro/VulnerableSpringDataRest.svg)

## CVE-2017-7921
 An Improper Authentication issue was discovered in Hikvision DS-2CD2xx2F-I Series V5.2.0 build 140721 to V5.4.0 build 160530, DS-2CD2xx0F-I Series V5.2.0 build 140721 to V5.4.0 Build 160401, DS-2CD2xx2FWD Series V5.3.1 build 150410 to V5.4.4 Build 161125, DS-2CD4x2xFWD Series V5.2.0 build 140721 to V5.4.0 Build 160414, DS-2CD4xx5 Series V5.2.0 build 140721 to V5.4.0 Build 160421, DS-2DFx Series V5.2.0 build 140805 to V5.4.5 Build 160928, and DS-2CD63xx Series V5.0.9 build 140305 to V5.3.5 Build 160106 devices. The improper authentication vulnerability occurs when an application does not adequately or correctly authenticate users. This may allow a malicious user to escalate his or her privileges on the system and gain access to sensitive information.



- [https://github.com/jorhelp/Ingram](https://github.com/jorhelp/Ingram) :  ![starts](https://img.shields.io/github/stars/jorhelp/Ingram.svg) ![forks](https://img.shields.io/github/forks/jorhelp/Ingram.svg)

- [https://github.com/chrisjd20/hikvision_CVE-2017-7921_auth_bypass_config_decryptor](https://github.com/chrisjd20/hikvision_CVE-2017-7921_auth_bypass_config_decryptor) :  ![starts](https://img.shields.io/github/stars/chrisjd20/hikvision_CVE-2017-7921_auth_bypass_config_decryptor.svg) ![forks](https://img.shields.io/github/forks/chrisjd20/hikvision_CVE-2017-7921_auth_bypass_config_decryptor.svg)

- [https://github.com/JrDw0/CVE-2017-7921-EXP](https://github.com/JrDw0/CVE-2017-7921-EXP) :  ![starts](https://img.shields.io/github/stars/JrDw0/CVE-2017-7921-EXP.svg) ![forks](https://img.shields.io/github/forks/JrDw0/CVE-2017-7921-EXP.svg)

- [https://github.com/K3ysTr0K3R/CVE-2017-7921-EXPLOIT](https://github.com/K3ysTr0K3R/CVE-2017-7921-EXPLOIT) :  ![starts](https://img.shields.io/github/stars/K3ysTr0K3R/CVE-2017-7921-EXPLOIT.svg) ![forks](https://img.shields.io/github/forks/K3ysTr0K3R/CVE-2017-7921-EXPLOIT.svg)

- [https://github.com/BurnyMcDull/CVE-2017-7921](https://github.com/BurnyMcDull/CVE-2017-7921) :  ![starts](https://img.shields.io/github/stars/BurnyMcDull/CVE-2017-7921.svg) ![forks](https://img.shields.io/github/forks/BurnyMcDull/CVE-2017-7921.svg)

- [https://github.com/voidsshadows/Hikvision-City-Hunter](https://github.com/voidsshadows/Hikvision-City-Hunter) :  ![starts](https://img.shields.io/github/stars/voidsshadows/Hikvision-City-Hunter.svg) ![forks](https://img.shields.io/github/forks/voidsshadows/Hikvision-City-Hunter.svg)

- [https://github.com/MisakaMikato/cve-2017-7921-golang](https://github.com/MisakaMikato/cve-2017-7921-golang) :  ![starts](https://img.shields.io/github/stars/MisakaMikato/cve-2017-7921-golang.svg) ![forks](https://img.shields.io/github/forks/MisakaMikato/cve-2017-7921-golang.svg)

- [https://github.com/201646613/CVE-2017-7921](https://github.com/201646613/CVE-2017-7921) :  ![starts](https://img.shields.io/github/stars/201646613/CVE-2017-7921.svg) ![forks](https://img.shields.io/github/forks/201646613/CVE-2017-7921.svg)

- [https://github.com/D2550/CVE_2017_7921_EXP](https://github.com/D2550/CVE_2017_7921_EXP) :  ![starts](https://img.shields.io/github/stars/D2550/CVE_2017_7921_EXP.svg) ![forks](https://img.shields.io/github/forks/D2550/CVE_2017_7921_EXP.svg)

- [https://github.com/kooroshsanaei/HikVision-CVE-2017-7921](https://github.com/kooroshsanaei/HikVision-CVE-2017-7921) :  ![starts](https://img.shields.io/github/stars/kooroshsanaei/HikVision-CVE-2017-7921.svg) ![forks](https://img.shields.io/github/forks/kooroshsanaei/HikVision-CVE-2017-7921.svg)

- [https://github.com/Wyl-cmd/CVE-2017-7921-Research-Toolkit](https://github.com/Wyl-cmd/CVE-2017-7921-Research-Toolkit) :  ![starts](https://img.shields.io/github/stars/Wyl-cmd/CVE-2017-7921-Research-Toolkit.svg) ![forks](https://img.shields.io/github/forks/Wyl-cmd/CVE-2017-7921-Research-Toolkit.svg)

- [https://github.com/aengussong/hikvision_probe](https://github.com/aengussong/hikvision_probe) :  ![starts](https://img.shields.io/github/stars/aengussong/hikvision_probe.svg) ![forks](https://img.shields.io/github/forks/aengussong/hikvision_probe.svg)

- [https://github.com/krypton612/hikivision](https://github.com/krypton612/hikivision) :  ![starts](https://img.shields.io/github/stars/krypton612/hikivision.svg) ![forks](https://img.shields.io/github/forks/krypton612/hikivision.svg)

- [https://github.com/0xf3d0rq/CVE-2017-7921](https://github.com/0xf3d0rq/CVE-2017-7921) :  ![starts](https://img.shields.io/github/stars/0xf3d0rq/CVE-2017-7921.svg) ![forks](https://img.shields.io/github/forks/0xf3d0rq/CVE-2017-7921.svg)

- [https://github.com/KelvinWin10/CVE-2017-7921-rewrite](https://github.com/KelvinWin10/CVE-2017-7921-rewrite) :  ![starts](https://img.shields.io/github/stars/KelvinWin10/CVE-2017-7921-rewrite.svg) ![forks](https://img.shields.io/github/forks/KelvinWin10/CVE-2017-7921-rewrite.svg)

- [https://github.com/saaydmr/hikvision-exploiter](https://github.com/saaydmr/hikvision-exploiter) :  ![starts](https://img.shields.io/github/stars/saaydmr/hikvision-exploiter.svg) ![forks](https://img.shields.io/github/forks/saaydmr/hikvision-exploiter.svg)

- [https://github.com/GabrielAvls/CVE-2017-7921](https://github.com/GabrielAvls/CVE-2017-7921) :  ![starts](https://img.shields.io/github/stars/GabrielAvls/CVE-2017-7921.svg) ![forks](https://img.shields.io/github/forks/GabrielAvls/CVE-2017-7921.svg)

- [https://github.com/mverschu/CVE-2017-7921](https://github.com/mverschu/CVE-2017-7921) :  ![starts](https://img.shields.io/github/stars/mverschu/CVE-2017-7921.svg) ![forks](https://img.shields.io/github/forks/mverschu/CVE-2017-7921.svg)

- [https://github.com/b3pwn3d/CVE-2017-7921](https://github.com/b3pwn3d/CVE-2017-7921) :  ![starts](https://img.shields.io/github/stars/b3pwn3d/CVE-2017-7921.svg) ![forks](https://img.shields.io/github/forks/b3pwn3d/CVE-2017-7921.svg)

- [https://github.com/inj3ction/CVE-2017-7921-EXP](https://github.com/inj3ction/CVE-2017-7921-EXP) :  ![starts](https://img.shields.io/github/stars/inj3ction/CVE-2017-7921-EXP.svg) ![forks](https://img.shields.io/github/forks/inj3ction/CVE-2017-7921-EXP.svg)

- [https://github.com/lastvocher/Hikvision-CVE-2017-7921-decryptor](https://github.com/lastvocher/Hikvision-CVE-2017-7921-decryptor) :  ![starts](https://img.shields.io/github/stars/lastvocher/Hikvision-CVE-2017-7921-decryptor.svg) ![forks](https://img.shields.io/github/forks/lastvocher/Hikvision-CVE-2017-7921-decryptor.svg)

- [https://github.com/p4tq/hikvision_CVE-2017-7921_auth_bypass_config_decryptor](https://github.com/p4tq/hikvision_CVE-2017-7921_auth_bypass_config_decryptor) :  ![starts](https://img.shields.io/github/stars/p4tq/hikvision_CVE-2017-7921_auth_bypass_config_decryptor.svg) ![forks](https://img.shields.io/github/forks/p4tq/hikvision_CVE-2017-7921_auth_bypass_config_decryptor.svg)

- [https://github.com/AnonkiGroup/AnonHik](https://github.com/AnonkiGroup/AnonHik) :  ![starts](https://img.shields.io/github/stars/AnonkiGroup/AnonHik.svg) ![forks](https://img.shields.io/github/forks/AnonkiGroup/AnonHik.svg)

## CVE-2017-7525
 A deserialization flaw was discovered in the jackson-databind, versions before 2.6.7.1, 2.7.9.1 and 2.8.9, which could allow an unauthenticated user to perform code execution by sending the maliciously crafted input to the readValue method of the ObjectMapper.



- [https://github.com/SecureSkyTechnology/study-struts2-s2-054_055-jackson-cve-2017-7525_cve-2017-15095](https://github.com/SecureSkyTechnology/study-struts2-s2-054_055-jackson-cve-2017-7525_cve-2017-15095) :  ![starts](https://img.shields.io/github/stars/SecureSkyTechnology/study-struts2-s2-054_055-jackson-cve-2017-7525_cve-2017-15095.svg) ![forks](https://img.shields.io/github/forks/SecureSkyTechnology/study-struts2-s2-054_055-jackson-cve-2017-7525_cve-2017-15095.svg)

- [https://github.com/JavanXD/Demo-Exploit-Jackson-RCE](https://github.com/JavanXD/Demo-Exploit-Jackson-RCE) :  ![starts](https://img.shields.io/github/stars/JavanXD/Demo-Exploit-Jackson-RCE.svg) ![forks](https://img.shields.io/github/forks/JavanXD/Demo-Exploit-Jackson-RCE.svg)

- [https://github.com/Ingenuity-Fainting-Goats/CVE-2017-7525-Jackson-Deserialization-Lab](https://github.com/Ingenuity-Fainting-Goats/CVE-2017-7525-Jackson-Deserialization-Lab) :  ![starts](https://img.shields.io/github/stars/Ingenuity-Fainting-Goats/CVE-2017-7525-Jackson-Deserialization-Lab.svg) ![forks](https://img.shields.io/github/forks/Ingenuity-Fainting-Goats/CVE-2017-7525-Jackson-Deserialization-Lab.svg)

- [https://github.com/Dannners/jackson-deserialization-2017-7525](https://github.com/Dannners/jackson-deserialization-2017-7525) :  ![starts](https://img.shields.io/github/stars/Dannners/jackson-deserialization-2017-7525.svg) ![forks](https://img.shields.io/github/forks/Dannners/jackson-deserialization-2017-7525.svg)

- [https://github.com/Nazicc/S2-055](https://github.com/Nazicc/S2-055) :  ![starts](https://img.shields.io/github/stars/Nazicc/S2-055.svg) ![forks](https://img.shields.io/github/forks/Nazicc/S2-055.svg)

## CVE-2017-7376
 Buffer overflow in libxml2 allows remote attackers to execute arbitrary code by leveraging an incorrect limit for port values when handling redirects.



- [https://github.com/brahmstaedt/libxml2-exploit](https://github.com/brahmstaedt/libxml2-exploit) :  ![starts](https://img.shields.io/github/stars/brahmstaedt/libxml2-exploit.svg) ![forks](https://img.shields.io/github/forks/brahmstaedt/libxml2-exploit.svg)

## CVE-2017-7047
 An issue was discovered in certain Apple products. iOS before 10.3.3 is affected. macOS before 10.12.6 is affected. tvOS before 10.2.2 is affected. watchOS before 3.2.3 is affected. The issue involves the "libxpc" component. It allows attackers to execute arbitrary code in a privileged context or cause a denial of service (memory corruption) via a crafted app.



- [https://github.com/JosephShenton/Triple_Fetch-Kernel-Creds](https://github.com/JosephShenton/Triple_Fetch-Kernel-Creds) :  ![starts](https://img.shields.io/github/stars/JosephShenton/Triple_Fetch-Kernel-Creds.svg) ![forks](https://img.shields.io/github/forks/JosephShenton/Triple_Fetch-Kernel-Creds.svg)

- [https://github.com/q1f3/Triple_fetch](https://github.com/q1f3/Triple_fetch) :  ![starts](https://img.shields.io/github/stars/q1f3/Triple_fetch.svg) ![forks](https://img.shields.io/github/forks/q1f3/Triple_fetch.svg)

## CVE-2017-6206
 D-Link DGS-1510-28XMP, DGS-1510-28X, DGS-1510-52X, DGS-1510-52, DGS-1510-28P, DGS-1510-28, and DGS-1510-20 Websmart devices with firmware before 1.31.B003 allow attackers to conduct Unauthenticated Information Disclosure attacks via unspecified vectors.



- [https://github.com/varangamin/CVE-2017-6206](https://github.com/varangamin/CVE-2017-6206) :  ![starts](https://img.shields.io/github/stars/varangamin/CVE-2017-6206.svg) ![forks](https://img.shields.io/github/forks/varangamin/CVE-2017-6206.svg)

## CVE-2017-6079
 The HTTP web-management application on Edgewater Networks Edgemarc appliances has a hidden page that allows for user-defined commands such as specific iptables routes, etc., to be set. You can use this page as a web shell essentially to execute commands, though you get no feedback client-side from the web application: if the command is valid, it executes. An example is the wget command. The page that allows this has been confirmed in firmware as old as 2006.



- [https://github.com/MostafaSoliman/CVE-2017-6079-Blind-Command-Injection-In-Edgewater-Edgemarc-Devices-Exploit](https://github.com/MostafaSoliman/CVE-2017-6079-Blind-Command-Injection-In-Edgewater-Edgemarc-Devices-Exploit) :  ![starts](https://img.shields.io/github/stars/MostafaSoliman/CVE-2017-6079-Blind-Command-Injection-In-Edgewater-Edgemarc-Devices-Exploit.svg) ![forks](https://img.shields.io/github/forks/MostafaSoliman/CVE-2017-6079-Blind-Command-Injection-In-Edgewater-Edgemarc-Devices-Exploit.svg)

## CVE-2017-5954
 An issue was discovered in the serialize-to-js package 0.5.0 for Node.js. Untrusted data passed into the deserialize() function can be exploited to achieve arbitrary code execution by passing a JavaScript Object with an Immediately Invoked Function Expression (IIFE).



- [https://github.com/ossf-cve-benchmark/CVE-2017-5954](https://github.com/ossf-cve-benchmark/CVE-2017-5954) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-5954.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-5954.svg)

## CVE-2017-5941
 An issue was discovered in the node-serialize package 0.0.4 for Node.js. Untrusted data passed into the unserialize() function can be exploited to achieve arbitrary code execution by passing a JavaScript Object with an Immediately Invoked Function Expression (IIFE).



- [https://github.com/rodolfomarianocy/nodeserial](https://github.com/rodolfomarianocy/nodeserial) :  ![starts](https://img.shields.io/github/stars/rodolfomarianocy/nodeserial.svg) ![forks](https://img.shields.io/github/forks/rodolfomarianocy/nodeserial.svg)

- [https://github.com/uartu0/nodejshell](https://github.com/uartu0/nodejshell) :  ![starts](https://img.shields.io/github/stars/uartu0/nodejshell.svg) ![forks](https://img.shields.io/github/forks/uartu0/nodejshell.svg)

- [https://github.com/Cr4zyD14m0nd137/Lab-for-cve-2018-15133](https://github.com/Cr4zyD14m0nd137/Lab-for-cve-2018-15133) :  ![starts](https://img.shields.io/github/stars/Cr4zyD14m0nd137/Lab-for-cve-2018-15133.svg) ![forks](https://img.shields.io/github/forks/Cr4zyD14m0nd137/Lab-for-cve-2018-15133.svg)

- [https://github.com/turnernator1/Node.js-CVE-2017-5941](https://github.com/turnernator1/Node.js-CVE-2017-5941) :  ![starts](https://img.shields.io/github/stars/turnernator1/Node.js-CVE-2017-5941.svg) ![forks](https://img.shields.io/github/forks/turnernator1/Node.js-CVE-2017-5941.svg)

- [https://github.com/Frivolous-scholar/CVE-2017-5941-NodeJS-RCE](https://github.com/Frivolous-scholar/CVE-2017-5941-NodeJS-RCE) :  ![starts](https://img.shields.io/github/stars/Frivolous-scholar/CVE-2017-5941-NodeJS-RCE.svg) ![forks](https://img.shields.io/github/forks/Frivolous-scholar/CVE-2017-5941-NodeJS-RCE.svg)

- [https://github.com/kylew1004/cve-2017-5941-poc-docker-lab](https://github.com/kylew1004/cve-2017-5941-poc-docker-lab) :  ![starts](https://img.shields.io/github/stars/kylew1004/cve-2017-5941-poc-docker-lab.svg) ![forks](https://img.shields.io/github/forks/kylew1004/cve-2017-5941-poc-docker-lab.svg)

- [https://github.com/f41k0n/RCE-NodeJs](https://github.com/f41k0n/RCE-NodeJs) :  ![starts](https://img.shields.io/github/stars/f41k0n/RCE-NodeJs.svg) ![forks](https://img.shields.io/github/forks/f41k0n/RCE-NodeJs.svg)

## CVE-2017-5871
 Odoo Version = 8.0-20160726 and Version 9 is affected by: CWE-601: Open redirection. The impact is: obtain sensitive information (remote).



- [https://github.com/1337rokudenashi/Odoo-leq-8.0-20160726-and-9.0-Open-Redirect](https://github.com/1337rokudenashi/Odoo-leq-8.0-20160726-and-9.0-Open-Redirect) :  ![starts](https://img.shields.io/github/stars/1337rokudenashi/Odoo-leq-8.0-20160726-and-9.0-Open-Redirect.svg) ![forks](https://img.shields.io/github/forks/1337rokudenashi/Odoo-leq-8.0-20160726-and-9.0-Open-Redirect.svg)

## CVE-2017-5721
 Insufficient input validation in system firmware for Intel NUC7i3BNK, NUC7i3BNH, NUC7i5BNK, NUC7i5BNH, NUC7i7BNH versions BN0049 and below allows local attackers to execute arbitrary code via manipulation of memory.



- [https://github.com/embedi/smm_usbrt_poc](https://github.com/embedi/smm_usbrt_poc) :  ![starts](https://img.shields.io/github/stars/embedi/smm_usbrt_poc.svg) ![forks](https://img.shields.io/github/forks/embedi/smm_usbrt_poc.svg)

## CVE-2017-5715
 Systems with microprocessors utilizing speculative execution and indirect branch prediction may allow unauthorized disclosure of information to an attacker with local user access via a side-channel analysis.



- [https://github.com/speed47/spectre-meltdown-checker](https://github.com/speed47/spectre-meltdown-checker) :  ![starts](https://img.shields.io/github/stars/speed47/spectre-meltdown-checker.svg) ![forks](https://img.shields.io/github/forks/speed47/spectre-meltdown-checker.svg)

- [https://github.com/nsacyber/Hardware-and-Firmware-Security-Guidance](https://github.com/nsacyber/Hardware-and-Firmware-Security-Guidance) :  ![starts](https://img.shields.io/github/stars/nsacyber/Hardware-and-Firmware-Security-Guidance.svg) ![forks](https://img.shields.io/github/forks/nsacyber/Hardware-and-Firmware-Security-Guidance.svg)

- [https://github.com/Eugnis/spectre-attack](https://github.com/Eugnis/spectre-attack) :  ![starts](https://img.shields.io/github/stars/Eugnis/spectre-attack.svg) ![forks](https://img.shields.io/github/forks/Eugnis/spectre-attack.svg)

- [https://github.com/ionescu007/SpecuCheck](https://github.com/ionescu007/SpecuCheck) :  ![starts](https://img.shields.io/github/stars/ionescu007/SpecuCheck.svg) ![forks](https://img.shields.io/github/forks/ionescu007/SpecuCheck.svg)

- [https://github.com/Viralmaniar/In-Spectre-Meltdown](https://github.com/Viralmaniar/In-Spectre-Meltdown) :  ![starts](https://img.shields.io/github/stars/Viralmaniar/In-Spectre-Meltdown.svg) ![forks](https://img.shields.io/github/forks/Viralmaniar/In-Spectre-Meltdown.svg)

- [https://github.com/opsxcq/exploit-cve-2017-5715](https://github.com/opsxcq/exploit-cve-2017-5715) :  ![starts](https://img.shields.io/github/stars/opsxcq/exploit-cve-2017-5715.svg) ![forks](https://img.shields.io/github/forks/opsxcq/exploit-cve-2017-5715.svg)

- [https://github.com/mathse/meltdown-spectre-bios-list](https://github.com/mathse/meltdown-spectre-bios-list) :  ![starts](https://img.shields.io/github/stars/mathse/meltdown-spectre-bios-list.svg) ![forks](https://img.shields.io/github/forks/mathse/meltdown-spectre-bios-list.svg)

- [https://github.com/00052/spectre-attack-example](https://github.com/00052/spectre-attack-example) :  ![starts](https://img.shields.io/github/stars/00052/spectre-attack-example.svg) ![forks](https://img.shields.io/github/forks/00052/spectre-attack-example.svg)

- [https://github.com/neuhalje/presentation_meltdown_spectre](https://github.com/neuhalje/presentation_meltdown_spectre) :  ![starts](https://img.shields.io/github/stars/neuhalje/presentation_meltdown_spectre.svg) ![forks](https://img.shields.io/github/forks/neuhalje/presentation_meltdown_spectre.svg)

- [https://github.com/ixtal23/spectreScope](https://github.com/ixtal23/spectreScope) :  ![starts](https://img.shields.io/github/stars/ixtal23/spectreScope.svg) ![forks](https://img.shields.io/github/forks/ixtal23/spectreScope.svg)

- [https://github.com/jarmouz/spectre_meltdown](https://github.com/jarmouz/spectre_meltdown) :  ![starts](https://img.shields.io/github/stars/jarmouz/spectre_meltdown.svg) ![forks](https://img.shields.io/github/forks/jarmouz/spectre_meltdown.svg)

- [https://github.com/EdwardOwusuAdjei/Spectre-PoC](https://github.com/EdwardOwusuAdjei/Spectre-PoC) :  ![starts](https://img.shields.io/github/stars/EdwardOwusuAdjei/Spectre-PoC.svg) ![forks](https://img.shields.io/github/forks/EdwardOwusuAdjei/Spectre-PoC.svg)

- [https://github.com/gonoph/ansible-meltdown-spectre](https://github.com/gonoph/ansible-meltdown-spectre) :  ![starts](https://img.shields.io/github/stars/gonoph/ansible-meltdown-spectre.svg) ![forks](https://img.shields.io/github/forks/gonoph/ansible-meltdown-spectre.svg)

- [https://github.com/miglen/Awesome-Meltdown-Spectre](https://github.com/miglen/Awesome-Meltdown-Spectre) :  ![starts](https://img.shields.io/github/stars/miglen/Awesome-Meltdown-Spectre.svg) ![forks](https://img.shields.io/github/forks/miglen/Awesome-Meltdown-Spectre.svg)

- [https://github.com/pedrolucasoliva/spectre-attack-demo](https://github.com/pedrolucasoliva/spectre-attack-demo) :  ![starts](https://img.shields.io/github/stars/pedrolucasoliva/spectre-attack-demo.svg) ![forks](https://img.shields.io/github/forks/pedrolucasoliva/spectre-attack-demo.svg)

- [https://github.com/MuhammadAnwaar/spectre](https://github.com/MuhammadAnwaar/spectre) :  ![starts](https://img.shields.io/github/stars/MuhammadAnwaar/spectre.svg) ![forks](https://img.shields.io/github/forks/MuhammadAnwaar/spectre.svg)

- [https://github.com/GalloLuigi/Analisi-CVE-2017-5715](https://github.com/GalloLuigi/Analisi-CVE-2017-5715) :  ![starts](https://img.shields.io/github/stars/GalloLuigi/Analisi-CVE-2017-5715.svg) ![forks](https://img.shields.io/github/forks/GalloLuigi/Analisi-CVE-2017-5715.svg)

- [https://github.com/GregAskew/SpeculativeExecutionAssessment](https://github.com/GregAskew/SpeculativeExecutionAssessment) :  ![starts](https://img.shields.io/github/stars/GregAskew/SpeculativeExecutionAssessment.svg) ![forks](https://img.shields.io/github/forks/GregAskew/SpeculativeExecutionAssessment.svg)

- [https://github.com/plyrthn/CiscoSpectreTakeover](https://github.com/plyrthn/CiscoSpectreTakeover) :  ![starts](https://img.shields.io/github/stars/plyrthn/CiscoSpectreTakeover.svg) ![forks](https://img.shields.io/github/forks/plyrthn/CiscoSpectreTakeover.svg)

- [https://github.com/kevincoakley/puppet-spectre_meltdown](https://github.com/kevincoakley/puppet-spectre_meltdown) :  ![starts](https://img.shields.io/github/stars/kevincoakley/puppet-spectre_meltdown.svg) ![forks](https://img.shields.io/github/forks/kevincoakley/puppet-spectre_meltdown.svg)

## CVE-2017-5693
 Firmware in the Intel Puma 5, 6, and 7 Series might experience resource depletion or timeout, which allows a network attacker to create a denial of service via crafted network traffic.



- [https://github.com/LunNova/Puma6Fail](https://github.com/LunNova/Puma6Fail) :  ![starts](https://img.shields.io/github/stars/LunNova/Puma6Fail.svg) ![forks](https://img.shields.io/github/forks/LunNova/Puma6Fail.svg)

## CVE-2017-5521
 An issue was discovered on NETGEAR R8500, R8300, R7000, R6400, R7300, R7100LG, R6300v2, WNDR3400v3, WNR3500Lv2, R6250, R6700, R6900, and R8000 devices. They are prone to password disclosure via simple crafted requests to the web management server. The bug is exploitable remotely if the remote management option is set, and can also be exploited given access to the router over LAN or WLAN. When trying to access the web panel, a user is asked to authenticate; if the authentication is canceled and password recovery is not enabled, the user is redirected to a page that exposes a password recovery token. If a user supplies the correct token to the page /passwordrecovered.cgi?id=TOKEN (and password recovery is not enabled), they will receive the admin password for the router. If password recovery is set the exploit will fail, as it will ask the user for the recovery questions that were previously set when enabling that feature. This is persistent (even after disabling the recovery option, the exploit will fail) because the router will ask for the security questions.



- [https://github.com/lilloX/routerPWN](https://github.com/lilloX/routerPWN) :  ![starts](https://img.shields.io/github/stars/lilloX/routerPWN.svg) ![forks](https://img.shields.io/github/forks/lilloX/routerPWN.svg)

## CVE-2017-5487
 wp-includes/rest-api/endpoints/class-wp-rest-users-controller.php in the REST API implementation in WordPress 4.7 before 4.7.1 does not properly restrict listings of post authors, which allows remote attackers to obtain sensitive information via a wp-json/wp/v2/users request.



- [https://github.com/K3ysTr0K3R/CVE-2017-5487-EXPLOIT](https://github.com/K3ysTr0K3R/CVE-2017-5487-EXPLOIT) :  ![starts](https://img.shields.io/github/stars/K3ysTr0K3R/CVE-2017-5487-EXPLOIT.svg) ![forks](https://img.shields.io/github/forks/K3ysTr0K3R/CVE-2017-5487-EXPLOIT.svg)

- [https://github.com/anx0ing/Wordpress_Brute](https://github.com/anx0ing/Wordpress_Brute) :  ![starts](https://img.shields.io/github/stars/anx0ing/Wordpress_Brute.svg) ![forks](https://img.shields.io/github/forks/anx0ing/Wordpress_Brute.svg)

- [https://github.com/patilkr/wp-CVE-2017-5487-exploit](https://github.com/patilkr/wp-CVE-2017-5487-exploit) :  ![starts](https://img.shields.io/github/stars/patilkr/wp-CVE-2017-5487-exploit.svg) ![forks](https://img.shields.io/github/forks/patilkr/wp-CVE-2017-5487-exploit.svg)

- [https://github.com/GeunSam2/CVE-2017-5487](https://github.com/GeunSam2/CVE-2017-5487) :  ![starts](https://img.shields.io/github/stars/GeunSam2/CVE-2017-5487.svg) ![forks](https://img.shields.io/github/forks/GeunSam2/CVE-2017-5487.svg)

- [https://github.com/R3K1NG/wpUsersScan](https://github.com/R3K1NG/wpUsersScan) :  ![starts](https://img.shields.io/github/stars/R3K1NG/wpUsersScan.svg) ![forks](https://img.shields.io/github/forks/R3K1NG/wpUsersScan.svg)

- [https://github.com/teambugsbunny/wpUsersScan](https://github.com/teambugsbunny/wpUsersScan) :  ![starts](https://img.shields.io/github/stars/teambugsbunny/wpUsersScan.svg) ![forks](https://img.shields.io/github/forks/teambugsbunny/wpUsersScan.svg)

- [https://github.com/tpdlshdmlrkfmcla/cve-2017-5487](https://github.com/tpdlshdmlrkfmcla/cve-2017-5487) :  ![starts](https://img.shields.io/github/stars/tpdlshdmlrkfmcla/cve-2017-5487.svg) ![forks](https://img.shields.io/github/forks/tpdlshdmlrkfmcla/cve-2017-5487.svg)

- [https://github.com/ndr-repo/CVE-2017-5487](https://github.com/ndr-repo/CVE-2017-5487) :  ![starts](https://img.shields.io/github/stars/ndr-repo/CVE-2017-5487.svg) ![forks](https://img.shields.io/github/forks/ndr-repo/CVE-2017-5487.svg)

- [https://github.com/SeasonLeague/CVE-2017-5487](https://github.com/SeasonLeague/CVE-2017-5487) :  ![starts](https://img.shields.io/github/stars/SeasonLeague/CVE-2017-5487.svg) ![forks](https://img.shields.io/github/forks/SeasonLeague/CVE-2017-5487.svg)

- [https://github.com/dream434/CVE-2017-5487](https://github.com/dream434/CVE-2017-5487) :  ![starts](https://img.shields.io/github/stars/dream434/CVE-2017-5487.svg) ![forks](https://img.shields.io/github/forks/dream434/CVE-2017-5487.svg)

- [https://github.com/zkhalidul/GrabberWP-CVE-2017-5487](https://github.com/zkhalidul/GrabberWP-CVE-2017-5487) :  ![starts](https://img.shields.io/github/stars/zkhalidul/GrabberWP-CVE-2017-5487.svg) ![forks](https://img.shields.io/github/forks/zkhalidul/GrabberWP-CVE-2017-5487.svg)

## CVE-2017-5223
 An issue was discovered in PHPMailer before 5.2.22. PHPMailer's msgHTML method applies transformations to an HTML document to make it usable as an email message body. One of the transformations is to convert relative image URLs into attachments using a script-provided base directory. If no base directory is provided, it resolves to /, meaning that relative image URLs get treated as absolute local file paths and added as attachments. To form a remote vulnerability, the msgHTML method must be called, passed an unfiltered, user-supplied HTML document, and must not set a base directory.



- [https://github.com/cscli/CVE-2017-5223](https://github.com/cscli/CVE-2017-5223) :  ![starts](https://img.shields.io/github/stars/cscli/CVE-2017-5223.svg) ![forks](https://img.shields.io/github/forks/cscli/CVE-2017-5223.svg)

## CVE-2017-5123
 Insufficient data validation in waitid allowed an user to escape sandboxes on Linux.



- [https://github.com/c3r34lk1ll3r/CVE-2017-5123](https://github.com/c3r34lk1ll3r/CVE-2017-5123) :  ![starts](https://img.shields.io/github/stars/c3r34lk1ll3r/CVE-2017-5123.svg) ![forks](https://img.shields.io/github/forks/c3r34lk1ll3r/CVE-2017-5123.svg)

- [https://github.com/0x5068656e6f6c/CVE-2017-5123](https://github.com/0x5068656e6f6c/CVE-2017-5123) :  ![starts](https://img.shields.io/github/stars/0x5068656e6f6c/CVE-2017-5123.svg) ![forks](https://img.shields.io/github/forks/0x5068656e6f6c/CVE-2017-5123.svg)

- [https://github.com/Synacktiv-contrib/exploiting-cve-2017-5123](https://github.com/Synacktiv-contrib/exploiting-cve-2017-5123) :  ![starts](https://img.shields.io/github/stars/Synacktiv-contrib/exploiting-cve-2017-5123.svg) ![forks](https://img.shields.io/github/forks/Synacktiv-contrib/exploiting-cve-2017-5123.svg)

- [https://github.com/FloatingGuy/CVE-2017-5123](https://github.com/FloatingGuy/CVE-2017-5123) :  ![starts](https://img.shields.io/github/stars/FloatingGuy/CVE-2017-5123.svg) ![forks](https://img.shields.io/github/forks/FloatingGuy/CVE-2017-5123.svg)

- [https://github.com/echo-devim/exploit_linux_kernel4.13](https://github.com/echo-devim/exploit_linux_kernel4.13) :  ![starts](https://img.shields.io/github/stars/echo-devim/exploit_linux_kernel4.13.svg) ![forks](https://img.shields.io/github/forks/echo-devim/exploit_linux_kernel4.13.svg)

- [https://github.com/teawater/CVE-2017-5123](https://github.com/teawater/CVE-2017-5123) :  ![starts](https://img.shields.io/github/stars/teawater/CVE-2017-5123.svg) ![forks](https://img.shields.io/github/forks/teawater/CVE-2017-5123.svg)

- [https://github.com/NabilBoudra/cve-2017-5123](https://github.com/NabilBoudra/cve-2017-5123) :  ![starts](https://img.shields.io/github/stars/NabilBoudra/cve-2017-5123.svg) ![forks](https://img.shields.io/github/forks/NabilBoudra/cve-2017-5123.svg)

- [https://github.com/h1bAna/CVE-2017-5123](https://github.com/h1bAna/CVE-2017-5123) :  ![starts](https://img.shields.io/github/stars/h1bAna/CVE-2017-5123.svg) ![forks](https://img.shields.io/github/forks/h1bAna/CVE-2017-5123.svg)

## CVE-2017-4878
 DO NOT USE THIS CANDIDATE NUMBER.  ConsultIDs: none.  Reason: This candidate was in a CNA pool that was not assigned to any issues during 2017.  Notes: none



- [https://github.com/brianwrf/CVE-2017-4878-Samples](https://github.com/brianwrf/CVE-2017-4878-Samples) :  ![starts](https://img.shields.io/github/stars/brianwrf/CVE-2017-4878-Samples.svg) ![forks](https://img.shields.io/github/forks/brianwrf/CVE-2017-4878-Samples.svg)

## CVE-2017-3066
 Adobe ColdFusion 2016 Update 3 and earlier, ColdFusion 11 update 11 and earlier, ColdFusion 10 Update 22 and earlier have a Java deserialization vulnerability in the Apache BlazeDS library. Successful exploitation could lead to arbitrary code execution.



- [https://github.com/codewhitesec/ColdFusionPwn](https://github.com/codewhitesec/ColdFusionPwn) :  ![starts](https://img.shields.io/github/stars/codewhitesec/ColdFusionPwn.svg) ![forks](https://img.shields.io/github/forks/codewhitesec/ColdFusionPwn.svg)

- [https://github.com/cucadili/CVE-2017-3066](https://github.com/cucadili/CVE-2017-3066) :  ![starts](https://img.shields.io/github/stars/cucadili/CVE-2017-3066.svg) ![forks](https://img.shields.io/github/forks/cucadili/CVE-2017-3066.svg)

## CVE-2017-3000
 Adobe Flash Player versions 24.0.0.221 and earlier have a vulnerability in the random number generator used for constant blinding. Successful exploitation could lead to information disclosure.



- [https://github.com/dangokyo/CVE-2017-3000](https://github.com/dangokyo/CVE-2017-3000) :  ![starts](https://img.shields.io/github/stars/dangokyo/CVE-2017-3000.svg) ![forks](https://img.shields.io/github/forks/dangokyo/CVE-2017-3000.svg)

## CVE-2017-2824
 An exploitable code execution vulnerability exists in the trapper command functionality of Zabbix Server 2.4.X. A specially crafted set of packets can cause a command injection resulting in remote code execution. An attacker can make requests from an active Zabbix Proxy to trigger this vulnerability.



- [https://github.com/listenquiet/cve-2017-2824-reverse-shell](https://github.com/listenquiet/cve-2017-2824-reverse-shell) :  ![starts](https://img.shields.io/github/stars/listenquiet/cve-2017-2824-reverse-shell.svg) ![forks](https://img.shields.io/github/forks/listenquiet/cve-2017-2824-reverse-shell.svg)

## CVE-2017-2671
 The ping_unhash function in net/ipv4/ping.c in the Linux kernel through 4.10.8 is too late in obtaining a certain lock and consequently cannot ensure that disconnect function calls are safe, which allows local users to cause a denial of service (panic) by leveraging access to the protocol value of IPPROTO_ICMP in a socket system call.



- [https://github.com/homjxi0e/CVE-2017-2671](https://github.com/homjxi0e/CVE-2017-2671) :  ![starts](https://img.shields.io/github/stars/homjxi0e/CVE-2017-2671.svg) ![forks](https://img.shields.io/github/forks/homjxi0e/CVE-2017-2671.svg)

## CVE-2017-2666
 It was discovered in Undertow that the code that parsed the HTTP request line permitted invalid characters. This could be exploited, in conjunction with a proxy that also permitted the invalid characters but with a different interpretation, to inject data into the HTTP response. By manipulating the HTTP response the attacker could poison a web-cache, perform an XSS attack, or obtain sensitive information from requests other than their own.



- [https://github.com/tafamace/CVE-2017-2666](https://github.com/tafamace/CVE-2017-2666) :  ![starts](https://img.shields.io/github/stars/tafamace/CVE-2017-2666.svg) ![forks](https://img.shields.io/github/forks/tafamace/CVE-2017-2666.svg)

## CVE-2017-2636
 Race condition in drivers/tty/n_hdlc.c in the Linux kernel through 4.10.1 allows local users to gain privileges or cause a denial of service (double free) by setting the HDLC line discipline.



- [https://github.com/alexzorin/cve-2017-2636-el](https://github.com/alexzorin/cve-2017-2636-el) :  ![starts](https://img.shields.io/github/stars/alexzorin/cve-2017-2636-el.svg) ![forks](https://img.shields.io/github/forks/alexzorin/cve-2017-2636-el.svg)

## CVE-2017-2370
 An issue was discovered in certain Apple products. iOS before 10.2.1 is affected. macOS before 10.12.3 is affected. tvOS before 10.1.1 is affected. watchOS before 3.1.3 is affected. The issue involves the "Kernel" component. It allows attackers to execute arbitrary code in a privileged context or cause a denial of service (buffer overflow) via a crafted app.



- [https://github.com/Peterpan0927/CVE-2017-2370](https://github.com/Peterpan0927/CVE-2017-2370) :  ![starts](https://img.shields.io/github/stars/Peterpan0927/CVE-2017-2370.svg) ![forks](https://img.shields.io/github/forks/Peterpan0927/CVE-2017-2370.svg)

- [https://github.com/Rootkitsmm-zz/extra_recipe-iOS-10.2](https://github.com/Rootkitsmm-zz/extra_recipe-iOS-10.2) :  ![starts](https://img.shields.io/github/stars/Rootkitsmm-zz/extra_recipe-iOS-10.2.svg) ![forks](https://img.shields.io/github/forks/Rootkitsmm-zz/extra_recipe-iOS-10.2.svg)

- [https://github.com/ldebug/extra_recipe](https://github.com/ldebug/extra_recipe) :  ![starts](https://img.shields.io/github/stars/ldebug/extra_recipe.svg) ![forks](https://img.shields.io/github/forks/ldebug/extra_recipe.svg)

- [https://github.com/maximehip/extra_recipe](https://github.com/maximehip/extra_recipe) :  ![starts](https://img.shields.io/github/stars/maximehip/extra_recipe.svg) ![forks](https://img.shields.io/github/forks/maximehip/extra_recipe.svg)

## CVE-2017-2027
 DO NOT USE THIS CANDIDATE NUMBER.  ConsultIDs: none.  Reason: This candidate was in a CNA pool that was not assigned to any issues during 2017.  Notes: none



- [https://github.com/ghhubin/weblogic_cve2017-20271](https://github.com/ghhubin/weblogic_cve2017-20271) :  ![starts](https://img.shields.io/github/stars/ghhubin/weblogic_cve2017-20271.svg) ![forks](https://img.shields.io/github/forks/ghhubin/weblogic_cve2017-20271.svg)

## CVE-2017-0931
 html-janitor node module suffers from a Cross-Site Scripting (XSS) vulnerability via clean() accepting user-controlled values.



- [https://github.com/ossf-cve-benchmark/CVE-2017-0931](https://github.com/ossf-cve-benchmark/CVE-2017-0931) :  ![starts](https://img.shields.io/github/stars/ossf-cve-benchmark/CVE-2017-0931.svg) ![forks](https://img.shields.io/github/forks/ossf-cve-benchmark/CVE-2017-0931.svg)

## CVE-2017-0781
 A remote code execution vulnerability in the Android system (bluetooth). Product: Android. Versions: 4.4.4, 5.0.2, 5.1.1, 6.0, 6.0.1, 7.0, 7.1.1, 7.1.2, 8.0. Android ID: A-63146105.



- [https://github.com/ojasookert/CVE-2017-0781](https://github.com/ojasookert/CVE-2017-0781) :  ![starts](https://img.shields.io/github/stars/ojasookert/CVE-2017-0781.svg) ![forks](https://img.shields.io/github/forks/ojasookert/CVE-2017-0781.svg)

- [https://github.com/CrackSoft900/Blue-Borne](https://github.com/CrackSoft900/Blue-Borne) :  ![starts](https://img.shields.io/github/stars/CrackSoft900/Blue-Borne.svg) ![forks](https://img.shields.io/github/forks/CrackSoft900/Blue-Borne.svg)

- [https://github.com/X3eRo0/android712-blueborne](https://github.com/X3eRo0/android712-blueborne) :  ![starts](https://img.shields.io/github/stars/X3eRo0/android712-blueborne.svg) ![forks](https://img.shields.io/github/forks/X3eRo0/android712-blueborne.svg)

- [https://github.com/DamianSuess/Learn.BlueJam](https://github.com/DamianSuess/Learn.BlueJam) :  ![starts](https://img.shields.io/github/stars/DamianSuess/Learn.BlueJam.svg) ![forks](https://img.shields.io/github/forks/DamianSuess/Learn.BlueJam.svg)

- [https://github.com/mjancek/BlueborneDetection](https://github.com/mjancek/BlueborneDetection) :  ![starts](https://img.shields.io/github/stars/mjancek/BlueborneDetection.svg) ![forks](https://img.shields.io/github/forks/mjancek/BlueborneDetection.svg)

- [https://github.com/CarlosDelRosario7/sploit-bX](https://github.com/CarlosDelRosario7/sploit-bX) :  ![starts](https://img.shields.io/github/stars/CarlosDelRosario7/sploit-bX.svg) ![forks](https://img.shields.io/github/forks/CarlosDelRosario7/sploit-bX.svg)

## CVE-2017-0505
 An elevation of privilege vulnerability in MediaTek components, including the M4U driver, sound driver, touchscreen driver, GPU driver, and Command Queue driver, could enable a local malicious application to execute arbitrary code within the context of the kernel. This issue is rated as Critical due to the possibility of a local permanent device compromise, which may require reflashing the operating system to repair the device. Product: Android. Versions: N/A. Android ID: A-31822282. References: M-ALPS02992041.



- [https://github.com/R0rt1z2/CVE-2017-0505-mtk](https://github.com/R0rt1z2/CVE-2017-0505-mtk) :  ![starts](https://img.shields.io/github/stars/R0rt1z2/CVE-2017-0505-mtk.svg) ![forks](https://img.shields.io/github/forks/R0rt1z2/CVE-2017-0505-mtk.svg)

## CVE-2017-0478
 A remote code execution vulnerability in the Framesequence library could enable an attacker using a specially crafted file to execute arbitrary code in the context of an unprivileged process. This issue is rated as High due to the possibility of remote code execution in an application that uses the Framesequence library. Product: Android. Versions: 5.0.2, 5.1.1, 6.0, 6.0.1, 7.0, 7.1.1. Android ID: A-33718716.



- [https://github.com/bingghost/CVE-2017-0478](https://github.com/bingghost/CVE-2017-0478) :  ![starts](https://img.shields.io/github/stars/bingghost/CVE-2017-0478.svg) ![forks](https://img.shields.io/github/forks/bingghost/CVE-2017-0478.svg)

- [https://github.com/likekabin/CVE-2017-0478](https://github.com/likekabin/CVE-2017-0478) :  ![starts](https://img.shields.io/github/stars/likekabin/CVE-2017-0478.svg) ![forks](https://img.shields.io/github/forks/likekabin/CVE-2017-0478.svg)

## CVE-2017-0411
 An elevation of privilege vulnerability in the Framework APIs could enable a local malicious application to execute arbitrary code within the context of a privileged process. This issue is rated as High because it could be used to gain local access to elevated capabilities, which are not normally accessible to a third-party application. Product: Android. Versions: 7.0, 7.1.1. Android ID: A-33042690.



- [https://github.com/lulusudoku/PoC](https://github.com/lulusudoku/PoC) :  ![starts](https://img.shields.io/github/stars/lulusudoku/PoC.svg) ![forks](https://img.shields.io/github/forks/lulusudoku/PoC.svg)

## CVE-2017-0204
 Microsoft Outlook 2007 SP3, Microsoft Outlook 2010 SP2, Microsoft Outlook 2013 SP1, and Microsoft Outlook 2016 allow remote attackers to bypass the Office Protected View via a specially crafted document, aka "Microsoft Office Security Feature Bypass Vulnerability."



- [https://github.com/ryhanson/CVE-2017-0204](https://github.com/ryhanson/CVE-2017-0204) :  ![starts](https://img.shields.io/github/stars/ryhanson/CVE-2017-0204.svg) ![forks](https://img.shields.io/github/forks/ryhanson/CVE-2017-0204.svg)

## CVE-2017-0145
 The SMBv1 server in Microsoft Windows Vista SP2; Windows Server 2008 SP2 and R2 SP1; Windows 7 SP1; Windows 8.1; Windows Server 2012 Gold and R2; Windows RT 8.1; and Windows 10 Gold, 1511, and 1607; and Windows Server 2016 allows remote attackers to execute arbitrary code via crafted packets, aka "Windows SMB Remote Code Execution Vulnerability." This vulnerability is different from those described in CVE-2017-0143, CVE-2017-0144, CVE-2017-0146, and CVE-2017-0148.



- [https://github.com/peterpt/eternal_scanner](https://github.com/peterpt/eternal_scanner) :  ![starts](https://img.shields.io/github/stars/peterpt/eternal_scanner.svg) ![forks](https://img.shields.io/github/forks/peterpt/eternal_scanner.svg)

- [https://github.com/MelonSmasher/chef_tissues](https://github.com/MelonSmasher/chef_tissues) :  ![starts](https://img.shields.io/github/stars/MelonSmasher/chef_tissues.svg) ![forks](https://img.shields.io/github/forks/MelonSmasher/chef_tissues.svg)

## CVE-2017-0108
 The Windows Graphics Component in Microsoft Office 2007 SP3; 2010 SP2; and Word Viewer; Skype for Business 2016; Lync 2013 SP1; Lync 2010; Live Meeting 2007; Silverlight 5; Windows Vista SP2; Windows Server 2008 SP2 and R2 SP1; and Windows 7 SP1 allows remote attackers to execute arbitrary code via a crafted web site, aka "Graphics Component Remote Code Execution Vulnerability." This vulnerability is different from that described in CVE-2017-0014.



- [https://github.com/homjxi0e/CVE-2017-0108](https://github.com/homjxi0e/CVE-2017-0108) :  ![starts](https://img.shields.io/github/stars/homjxi0e/CVE-2017-0108.svg) ![forks](https://img.shields.io/github/forks/homjxi0e/CVE-2017-0108.svg)

## CVE-2017-0089
 Uniscribe in Microsoft Windows Vista SP2, Windows Server 2008 SP2 and R2 SP1, and Windows 7 SP1 allows remote attackers to execute arbitrary code via a crafted web site, aka "Uniscribe Remote Code Execution Vulnerability." This vulnerability is different from those described in CVE-2017-0072, CVE-2017-0083, CVE-2017-0084, CVE-2017-0086, CVE-2017-0087, CVE-2017-0088, and CVE-2017-0090.



- [https://github.com/rainhawk13/Added-Pentest-Ground-to-vulnerable-websites-for-training](https://github.com/rainhawk13/Added-Pentest-Ground-to-vulnerable-websites-for-training) :  ![starts](https://img.shields.io/github/stars/rainhawk13/Added-Pentest-Ground-to-vulnerable-websites-for-training.svg) ![forks](https://img.shields.io/github/forks/rainhawk13/Added-Pentest-Ground-to-vulnerable-websites-for-training.svg)

## CVE-2017-0055
 Microsoft Internet Information Server (IIS) in Windows Vista SP2; Windows Server 2008 SP2 and R2; Windows 7 SP1; Windows 8.1; Windows Server 2012 Gold and R2; Windows RT 8.1; Windows 10 Gold, 1511, and 1607; and Windows Server 2016 allows remote attackers to perform cross-site scripting and run script with local user privileges via a crafted request, aka "Microsoft IIS Server XSS Elevation of Privilege Vulnerability."



- [https://github.com/NetJBS/CVE-2017-0055-PoC](https://github.com/NetJBS/CVE-2017-0055-PoC) :  ![starts](https://img.shields.io/github/stars/NetJBS/CVE-2017-0055-PoC.svg) ![forks](https://img.shields.io/github/forks/NetJBS/CVE-2017-0055-PoC.svg)
