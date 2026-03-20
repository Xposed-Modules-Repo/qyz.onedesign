# ⭐ OneDesign - OneUI 8.0 自定义增强框架

## 项目介绍

**OneDesign** 通过 Xposed Hook 技术在系统级别对多个应用进行定制，提供本地化支持、功能增强和系统优化。

支持的系统版本：**Android 16+ (OneUI 8.0+)**

---

## 核心功能模块

### 🌍 本地化与区域定制

#### 📱 来电显示与号码识别
- 港版系统来电归属地显示
- 号码识别与显示优化

#### 🎨 主题与视觉定制
- OneUI 主题切换与样式调整
- 系统主题颜色自定义
- 第三方应用主题适配

#### 📅 日历本地化
- 港版日历"智能节假日"支持
- 农历显示
- 本地假期识别与提醒
- **涉及应用**：日历 (Calendar)

#### 🌤️ 天气与地区
- 地区天气数据本地化
- 天气应用UI适配
- **涉及应用**：天气 (Weather)

---

### 🔧 系统功能增强

#### 📸 相机功能
- **关闭相机快门声音** - 港版机型必备功能
- 相机参数优化
- **涉及应用**：相机 (Camera)

#### 📞 通信应用
- **短信应用 (SMS)**
  - 短信记录本地存储（Room 数据库）
  - 短信归档和查询
  - 验证码提取

- **消息应用增强** (Message)
  - 消息处理优化
  
- **拨号器功能** (Samsung Dialer)
  - 通话界面定制
  - 联系人显示优化

#### ⏰ 时间相关
- **时钟应用** - 闹钟与计时器优化
- **提醒应用** (S Reminder) - 提醒显示增强
- **时间显示本地化**

#### 🎮 应用与娱乐
- **哔哩哔哩** (Bilibili) 
  - 播放参数优化
  - 界面适配

- **相册应用** (Gallery)
  - 相册管理增强
  
- **Game Tools** - 游戏工具增强
  
- **Photo Editor** - 照片编辑优化

#### ☁️ 云服务
- **Samsung Cloud** 优化与定制
- **自修复应用** (Self Repair) 增强

#### 🏠 系统应用
- **设置应用** - 软件版本显示为"官方"
- **主屏幕** (Home Screen) 定制
- **翻译应用** (Translate) 优化
- **Google Play 服务** (GMS) 集成增强

#### 🔐 安全与Knox保护
- **Knox 系统Hooks** 
  - Knox Matrix 集成
  - Samsung Keystore 兼容
  - Root 检测处理
  - Knox SDK 支持
  
- **Samsung Health** 与 Knox 兼容性
  
- **Secure Folder** 支持
  
- **Samsung Account** 认证优化
  
- **Quick Share** 功能增强

#### ⚡ 系统优化
- **降压超频支持** - 去除 SSRM WARNING 弹窗
- **框架级优化** (Framework Hook)
- **电源管理增强** (PowerEnhance Hook)
- **SystemUI 优化** (SystemUI Hook)
- **包管理器优化** (Package Manager Hook)
- **标志安全禁用** - 允许屏幕录制/截图
- **FCM 广播处理** (Google Cloud Messaging)
- **Android 7 特性** 支持

---

### 📊 数据管理与存储

#### SMS 功能模块
- 短信拦截与本地存储
- SQLite/Room 数据库管理
- 短信验证码提取器

#### 其他数据功能
- **设备信息管理** (MyDevice)
- **启动监控** (FreezeMonitor)
- **分区挂载** (Mount Feature)
- **AVB 验证** (AVB Feature)

---

### 🎯 边缘屏幕与快捷功能

#### 📱 Edge Screen (边屏功能)
- 边缘屏幕快捷面板
- 自定义快捷功能
- 快速启动支持

#### 🔔 系统事件处理
- 启动完成处理 (Boot Receiver)
- 重启事件处理 (Reboot Receiver)
- Edge 屏幕事件接收 (PayEdgeScreenReceiver)

---

## 技术架构

### 核心框架
- **Xposed Hook 框架** - 系统级别的应用定制
- **YukiHookAPI** - 简化的 Hook API 封装
- **Kotlin 2.3.20** - 最新 Kotlin 语言支持

### UI 框架
- **Jetpack Compose** - 现代化的声明式 UI 框架
- **HyperX Compose** - 自定义 Compose 组件库
- **MIUIX Navigation** - 高级导航支持
- **Material Design 3** - 现代设计规范

### 数据与存储
- **Android Room** - 类型安全的数据库访问
- **SharedPreferences** - 配置存储
- **SQLite** - 数据持久化

### 依赖注入
- **Hilt** - 编译时依赖注入框架
- **Provider** - 依赖提供者模式

### 其他关键库
- **Retrofit 3.0** - HTTP 网络请求
- **Coroutines** - 异步编程
- **Serialization** - JSON 序列化
- **DexKit** - DEX 文件分析
- **LSParanoid** - 代码混淆保护
- **libsu** - ROOT 权限处理

---

## 项目结构

