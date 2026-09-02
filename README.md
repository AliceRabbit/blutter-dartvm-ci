# blutter-dartvm-ci

用 GitHub Actions 的 windows-latest(MSVC)构建 [blutter](https://github.com/worawit/blutter)
所匹配的 Dart VM 与可执行文件,用于对 Flutter App 的 `libapp.so`(arm64)做静态分析。

- 手动触发(workflow_dispatch),参数:Dart 版本、快照哈希、blutter 源仓库
- 产物为 artifact:`blutter_dartvm<ver>_android_arm64.exe` + 运行所需 DLL
- 本仓库不包含任何 App 二进制文件,仅开源构建脚本
