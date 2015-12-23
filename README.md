# ss-switch

Introduce:
  For those people who have multiple Shadowsocks servers, this tool can easily switch your server setting.
  
Requirments:
  OS: Openwrt
  Package Dependency: openwrt-shadowsocks,python-mini
  
Installation:
  Copy the file "ss-switch" into directory "/usr/bin/"
  Add excute permission to the file(e.g. chmod +x ss-switch)
  Now you can type "ss-switch" in the command line to use this tool.
  
Instruction:
  At first,if your SS servers have common port and password,you can set default value for them by the command line "ss-switch setdefault"(e.g. ss-switch setdefault 1078 password).
  Use "ss-switch add" to add an entry for each SS servers.
  Use "ss-switch show" to show all the entries added.Each entry will be assigned a integer as its ID.
  Use "ss-switch use <ID>" to choose one entry to use.
  Use "ss-switch ping <ID>" to show the ping information of a SS server.
  Use "ss-switch delete <ID>" to delete an entry.
  
  You can also view this help information by typing "ss-switch -h".
