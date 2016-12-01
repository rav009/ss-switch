# ss-switch

##Introduce:
For those people who have multiple Shadowsocks servers, this tool can easily switch your SS server setting from one to another.

##Requirments:
- OS: Openwrt
- Package Dependency: openwrt-shadowsocks, python-mini

##Installation:
1. Copy the file "ss-switch" into directory "/usr/bin/".
2. Add excute permission to the file(e.g. chmod +x ss-switch).
3. Now you can type "ss-switch" in the command line to use this tool.

##Instruction:
- At first,if your SS servers have common port and password,you can set default value for them by the command line "ss-switch setdefault"(e.g. ss-switch setdefault 33078 password).
- Use "ss-switch add" to add an entry for each SS servers.
- Use "ss-switch show" to show the current SS status and all entries added.Each entry will be assigned a integer as its ID.
- Use "ss-switch use `<id>`" to choose one entry to use.
- Use "ss-switch ping `<id>`" to show the ping information of a SS server.
- Use "ss-switch delete `<id>`" to delete an entry.
- Use "ss-switch on" to turn on SS.
- Use "ss-switch off" to turn off SS.
- Use "ss-switch ip" to get the list of IPs allowed to access SS.
- Use "ss-switch allow `<ip>`" to allow certain IP to access SS.
- Use "ss-switch ban `<ip>`" to ban certain IP from the access of SS.
- You can also view this help information by typing "ss-switch -h".

