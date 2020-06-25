# MER1200Gv1
水星MER1200Gv1原厂编程器固件、原厂EEPROM、TP-Link Archer C5 v4移植固件

## 硬件规格
- **CPU** MT7620A
- **无线** MT7612EN
- **交换机** RTL8367S
- **RAM** 64M
- **Flash** 16M

与TP-Link Archer C5 v4几乎完全一致，刷机要用编程器。

参见：https://openwrt.org/toh/hwdata/tp-link/tp-link_archer_c5_v4

## Archer C5 v4移植固件
- 管理地址`192.168.0.1`
- 管理密码`admin`/`admin`
- 无线密码`12345670`
- 替换为MER1200G原厂EEPROM
- 加了个~~没卵用的~~telnet后门

telnet后门食用方法
  1. 登录后台
  2. 进入**Securiy** -> **Access Control**
  3. 打开**Access Control**开关
  4. 在**Devices in Blacklist**新增一项MAC地址为`EE-EE-EE-EE-EE-EE`的条目
  5. telnet管理地址，取得shell
