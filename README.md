# Hackintosh-Clover-EFI-ThinkPad-E430

联想 ThinkPad E430 黑苹果 EFI Clover 版

简单说明下:记得自己更换下 config.plist 中的 UUID

目前这个 Clover EFI 可以支持到 macOS Catalina 10.15.6 Beta版（19G60d），不支持最新的 macOS 11 Beta 版。

支持 ThinkPad E430 核显版的笔记本,这个型号的 ThinkPad 有好多款，配置基本相同，但我手头这款是企业集中采购的,只有核显没独立硬盘的版本,由于是老款笔记本，配置不够，加了内存换了SSD固态，如果你的硬件配置这方面跟我不同，应该也不影响启动。

基于 DSDT 和 SSDT 的方式修改的。Clover 里能不选的都空着了，好处是升级系统时直接过，不会出现这样那样的问题。

DSDT 和 SSDT 里面有包括扬声器声卡电池等方面的修改。

有线网卡没问题，无限网卡暂时不解决了，因为联想的本子锁 Bios，即使换无限网卡也需要焊 Bios 下来刷白名单，太麻烦，或者你也可以考虑某宝上购买个兼容黑苹果的 USB 无线网卡，缺点就是发热大，稳定性一般，不支持随航隔空投送之类，只能用来上上网而已。

亮度方面-无自动亮度调节，这本子屏幕亮度本来就不太高，没必要自动了，但可以手动调节，保持最亮而不存在关机后开机又变暗之类的问题。。。

声卡-没使用万能驱动，用的仿冒版驱动，比万能驱动更好，声音方面没问题，麦克风方面也没问题，也不存在插上耳机音响后左右声道有不响之类的问题。。。

电池-基本没问题。休眠方面可能有点小问题，自己测试下吧。具体懒得继续测试了。

CPU 变频方面也做过过修改了。没问题。不存在开机自检花屏之类的问题。添加了硬件状态监控驱动。

