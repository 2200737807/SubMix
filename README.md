# SubMix
### 📁 目录结构

```
SubMix/
├── 📁 app/                           # Next.js App Router
│   ├── 📁 api/
│   │   ├── convert/route.ts          # 配置转换 API
│   │   ├── proxy-config/route.ts     # 协议配置 API
│   │   ├── sub/route.ts              # 节点转换 API (类似 Sub Converter)
│   │   └── subscription/route.ts     # 订阅配置存储 API
│   ├── page.tsx                      # 主页面
│   ├── layout.tsx                    # 根布局
│   └── globals.css                   # 全局样式
├── 📁 components/                    # React 组件
│   ├── 📁 proxy/                     # 代理相关组件
│   │   ├── AddNodeCard.tsx           # 添加节点卡片
│   │   ├── NodeListCard.tsx          # 节点列表卡片
│   │   ├── EditNodeDialog.tsx        # 节点编辑对话框
│   │   ├── ConfigOptionsCard.tsx     # 配置选项卡片
│   │   ├── ConfigOutputCard.tsx      # 配置输出卡片
│   │   └── ProtocolSupportCard.tsx   # 协议支持说明卡片
│   └── 📁 ui/                        # shadcn/ui 基础组件
├── 📁 hooks/                         # 自定义 Hooks
│   ├── useProxyManagement.ts         # 代理管理 Hook
│   ├── useConfigGeneration.ts        # 配置生成 Hook
│   └── useEditConfig.ts              # 编辑配置 Hook
├── 📁 lib/                          # 核心库
│   ├── 📁 protocol-configs/          # 🔥 协议配置模块（新架构）
│   │   ├── 📁 base/                  # 基础库
│   │   │   ├── common-fields.ts      # 公共字段定义
│   │   │   ├── field-groups.ts       # 字段分组配置
│   │   │   └── field-types.ts        # 字段类型和选项
│   │   ├── 📁 protocols/             # 协议配置文件
│   │   │   ├── vless.config.ts       # VLESS 协议配置
│   │   │   ├── hysteria.config.ts    # Hysteria 协议配置
│   │   │   ├── hysteria2.config.ts   # Hysteria2 协议配置
│   │   │   ├── shadowsocks.config.ts # Shadowsocks 协议配置
│   │   │   └── trojan.config.ts      # Trojan 协议配置
│   │   ├── generator.ts              # 配置生成器
│   │   └── index.ts                  # 统一导出
│   ├── 📁 parsers/                   # 协议解析器
│   │   ├── base.ts                   # 解析器基类和接口
│   │   ├── vless.ts                  # VLESS 解析器
│   │   ├── hysteria.ts               # Hysteria 解析器
│   │   ├── hysteria2.ts              # Hysteria2 解析器
│   │   ├── shadowsocks.ts            # Shadowsocks 解析器
│   │   └── trojan.ts                 # Trojan 解析器
│   ├── proxy-parser.ts               # 解析器入口
│   ├── mihomo-config.ts              # Mihomo 配置生成器
│   └── utils.ts                      # 工具函数
├── 📁 types/                        # TypeScript 类型定义
│   └── proxy.ts                      # 代理相关类型
├── 📁 utils/                        # 工具模块
│   └── protocolUtils.ts              # 协议工具函数
└── 📁 public/                       # 静态资源
```

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## ⚠️ 免责声明

本工具仅用于学习和测试目的，请遵守当地法律法规。


## 🙏 鸣谢

- [Mihomo](https://github.com/MetaCubeX/mihomo) - 强大的代理内核
- [Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules) - 高质量规则集
- [shadcn/ui](https://ui.shadcn.com/) - 优秀的 UI 组件库
- [Next.js](https://nextjs.org/) - 现代化的 React 框架
