# Threat Modelling Frameworks

本仓库用于记录和实践网络安全中的 **Threat Modeling（威胁建模）** 方法，包括 STRIDE、LINDDUN、数据流图（DFD）以及常见安全威胁与缓解措施。

## 1. 项目目标

通过实际案例学习和掌握威胁建模的基本流程：

1. 理解系统架构
2. 识别资产（Assets）
3. 绘制数据流图（Data Flow Diagram, DFD）
4. 识别信任边界（Trust Boundary）
5. 使用威胁建模框架识别潜在风险
6. 分析攻击路径
7. 设计对应的安全缓解措施（Mitigation）

---

## 2. STRIDE Threat Model

STRIDE 是 Microsoft 提出的一种经典威胁建模方法。

| 类型 | 英文 | 主要安全问题 |
|---|---|---|
| S | Spoofing | 身份伪造 |
| T | Tampering | 数据篡改 |
| R | Repudiation | 行为抵赖 |
| I | Information Disclosure | 信息泄露 |
| D | Denial of Service | 拒绝服务 |
| E | Elevation of Privilege | 权限提升 |

可以使用 STRIDE 对系统中的：

- External Entity
- Process
- Data Store
- Data Flow
- Trust Boundary

进行系统化威胁分析。

---

## 3. Threat Modeling Process

基本威胁建模流程：

```text
System Understanding
        ↓
Architecture Design
        ↓
Data Flow Diagram
        ↓
Trust Boundary Analysis
        ↓
Threat Identification
        ↓
STRIDE Analysis
        ↓
Risk Assessment
        ↓
Security Mitigation
