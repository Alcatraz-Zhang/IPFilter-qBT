# IP Filter Converter

这是一个Python脚本,用于将IP地址列表转换为特定格式的IP过滤器文件。

## 功能

- 从BTN-Collected-Rules项目中订阅IP地址列表
- 将IPv4 CIDR转换为范围格式 (例如: 192.168.1.0/24 -> 192.168.1.1-192.168.1.254)
- 将IPv6地址转换为完整的展开格式
- 将IPv6 CIDR转换为范围格式
- 跳过无效的IP地址
- 生成名为 `ipfilter.dat` 的输出文件

## 使用方法

1. 确保您的系统上安装了Python 3。
2. 运行脚本:
   ```
   python ip-filter-converter.py
   ```
3. 脚本会生成一个名为 `ipfilter.dat` 的输出文件。

## 注意事项

- 脚本会自动跳过无效的IP地址。
- IPv4 CIDR会被转换为范围格式,但会排除网络地址和广播地址。
- IPv6地址会被转换为完整的展开格式。
- IPv6 CIDR会被转换为完整的展开格式的范围。
- 输出文件 `ipfilter.dat` 将被保存在与脚本相同的目录中。

## 贡献

欢迎提出改进建议或报告问题。

## 许可证

本项目采用 [MIT License](./LICENSE) 开源。