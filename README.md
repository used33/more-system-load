# Multi-Boot Project

这是一个用于实现多系统引导的项目，它提供了一种简单的方法，只需要把文件放入系统引导分区，并修改efi文件夹名称或修改conf文件配置信息，就可以在启动时选择不同的操作系统。

## 如何使用

要使用这个项目，你需要以下步骤：

- 准备一个包含多个操作系统的硬盘，例如Windows，Linux，MacOS等，确保每个操作系统都有一个独立的分区或者虚拟硬盘，并且至少有一个分区是EFI分区。
- 克隆或下载本项目到你的本地目录，然后将`multi-boot`文件夹复制到EFI分区的根目录下。
- 将每个操作系统的efi文件夹重命名为`os1`，`os2`，`os3`等，按照你想要的启动顺序排列，例如，如果你想要先启动Windows，再启动Linux，再启动MacOS，那么你可以将Windows的efi文件夹重命名为`os1`，Linux的efi文件夹重命名为`os2`，MacOS的efi文件夹重命名为`os3`。
- 修改`multi-boot\conf\multi-boot.conf`文件，根据你的实际情况填写每个操作系统的名称，例如：

```
[os1]
name = Windows
[os2]
name = Linux
[os3]
name = MacOS
```

- 重启你的电脑，然后在启动菜单中选择`multi-boot`选项，你就可以看到一个多系统引导界面，你可以用方向键和回车键来选择你想要启动的操作系统。

## 参考资料

以下是一些有用的参考资料，你可以通过它们来学习更多关于多系统引导的知识：

- [多系统引导的原理和实现](https://www.cnblogs.com/zhengyun_ustc/p/multiboot.html)
- [如何在同一台电脑上安装多个操作系统](https://www.howtogeek.com/187789/dual-booting-explained-how-you-can-have-multiple-operating-systems-on-your-computer/)
- [如何使用grub2配置多系统引导](https://www.linux.com/training-tutorials/how-configure-grub2-multiple-operating-systems/)

## 贡献者

这个项目是忠心的byby的，如果你有任何问题或建议，请联系。
