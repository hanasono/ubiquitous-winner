https://www.kali.org/news/kali-linux-in-the-windows-app-store/

Digest:

```
PS:> Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```
```
$ sudo apt-get update
$ sudo apt-get dist-upgrade
```
```
$ sudo apt-get update
$ sudo apt-get install metasploit-framework
```

---
Kali on Azure

add inbound rule for port 22 and home ip to allow ssh connection
---
dns

fierce -dns somedomain -wordlist somelist -threads 10

---
scan

nmap -vv -o -sS -A -p- P0 -oX test.xml 106.1**.**1.40

NSE
- auth：此类脚本使用暴力破解等技术找出目标系统上的认证信息。
- default：启用--sC 或者-A 选项时运行此类脚本。这类脚本同时具有下述特点：
  * 执行速度快；
  * 输出的信息有指导下一步操作的价值；
  * 输出信息内容丰富、形式简洁；
  * 必须可靠；
  * 不会侵入目标系统；
  * 能泄露信息给第三方。
- discovery：该类脚本用于探索网络。
- dos：该类脚本可能使目标系统拒绝服务，请谨慎使用。
- exploit：该类脚本利用目标系统的安全漏洞。在运行这类脚本之前，渗透测试人员需要获取被测单位的行动许可。
- external：该类脚本可能泄露信息给第三方。
- fuzzer：该类脚本用于对目标系统进行模糊测试。
- instrusive：该类脚本可能导致目标系统崩溃，或耗尽目标系统的所有资源。
- malware：该类脚本检査目标系统上是否存在恶意软件或后门。
- safe：该类脚本不会导致目标服务崩溃、拒绝服务且不利用漏洞。
- version：配合版本检测选项（-sV），这类脚本对目标系统的服务程序进行深入的版本检测。
- vuln：该类脚本可检测检査目标系统上的安全漏洞。
在Kali Linux系统中，Nmap脚本位于目录/usr/share/nmap/scripts。目前，Kali Linux收录的6.25版的Nmap带有430多个脚本。
在使用NSE脚本时，可以下命令行里使用下述选项。
- -sC 或--script=default：启动默认类NSE 脚本。
- --script <filename>|<category>|<directories>：根据指定的文件名、类别名、目录名，执行相应的脚本。
- --script-args <args>：这个选项用于给脚本指定参数。例如，在使用认证类脚本时，可通过这个选项指定用户名和密码。

- -d: enable debug mode to see log
---

vuln

https://www.exploit-db.com/
https://www.exploit-db.com/google-hacking-database/
http://www.openvas.org/

sqlmap

