### 修改系统配置
- 在搜索栏输入**cmd**, 右击**命令提示符**, 点击已管理员身份运行. 如图一所示:![图一](https://upload-images.jianshu.io/upload_images/10385410-3a8fc27b1af970e8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 分别复制以下两行指令到命令行窗口内, 点击回车运行, 结果如图二:
>REG ADD HKLM\SYSTEM\CurrentControlSet\Services\RasMan\Parameters /v ProhibitIpSec /t REG_DWORD /d 0x0 /f
>REG ADD HKLM\SYSTEM\CurrentControlSet\Services\PolicyAgent /v AssumeUDPEncapsulationContextOnSendRule /t REG_DWORD /d 0x2 /f

![图二](https://upload-images.jianshu.io/upload_images/10385410-22cd091e4bf370b3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 重启电脑让刚才修改的注册表生效

### 配置VPN连接
- 在**设置/网络和Internet/VPN**板块中点击**添加VPN连接**, 如图三所示
![图三](https://upload-images.jianshu.io/upload_images/10385410-a7c36c548cabc16a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 填写各项信息, 如图四, 点击保存
![图四](https://upload-images.jianshu.io/upload_images/10385410-7ed09977feec81d8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 在**设置/网络和Internet/状态**板块中点击**更改适配器选项**, 如图五所示
![图五](https://upload-images.jianshu.io/upload_images/10385410-9f0f75f61b6100c9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 右击你所新建的VPN连接, 选择**属性**, 选择属性面板上的**安全**, 如图六所示进行配置
![图六](https://upload-images.jianshu.io/upload_images/10385410-6ba50ec5ea27d6b5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 连接VPN
选择右下角的网络图标,  选择VPN连接, 点击**连接**即可, 如图7.
![图7](https://upload-images.jianshu.io/upload_images/10385410-cb2b1bde4046c20e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
