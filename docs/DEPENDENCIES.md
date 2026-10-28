# 编译依赖

- `libs/MainMenu-mc26.3-plugin-1.10.1-beta.1.jar`：compile/test only; full plugin JAR, not embedded；[来源](https://github.com/SWUST-Minecraft-Club/mcPlugin/tree/2ed15975fd633057321a52cc08b2de8e0d9a21fb/Minecraft-26_3-plugin/MainMenu)。SHA-256 见锁文件。
- `libs/arcmenu-api-3.2.0.jar`：compile only; external API; see upstream sources in docs/DEPENDENCIES.md；[来源](https://github.com/SWUST-Minecraft-Club/mcPlugin/tree/2ed15975fd633057321a52cc08b2de8e0d9a21fb/libs/arcmenu-api-3.2.0.jar)。SHA-256 见锁文件。

ArcMenu 官方文档：https://docs.myarc.icu ；API 继承原集成仓的固定编译输入，不分发运行时。


固定完整插件 JAR 仅用于编译和测试，不能作为精简 API JAR 宣传；运行时由服务器插件类加载器提供类，最终产品不嵌入这些依赖。更新时同时更新 Gradle 路径和锁文件。
