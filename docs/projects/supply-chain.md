---
AIGC:
    Label: "1"
    ContentProducer: 001191440300708461136T1XGW3
    ProduceID: 038f982d5cc69ead6143a5e970ea65d2_13ed3b98adb611f1b128525400f8a581
    ReservedCode1: XzBqPq8eSKPh3DXSvbdHHR4jTX5F1awN/3j63fHqFUJnVOVLpDWnzup/oBYc/2q902tCVR4AhA6WdlLxq6zVwWto3rZ8I5TPELtavglx6cd0Z8uTYMJL3nAx22QuT93GUDHJKG9J0U4DDE9PdsnEfkVAfUUGq+m5yahfsSBo31ZwiHpDSCGZauJDiH4=
    ContentPropagator: 001191440300708461136T1XGW3
    PropagateID: 038f982d5cc69ead6143a5e970ea65d2_13ed3b98adb611f1b128525400f8a581
    ReservedCode2: XzBqPq8eSKPh3DXSvbdHHR4jTX5F1awN/3j63fHqFUJnVOVLpDWnzup/oBYc/2q902tCVR4AhA6WdlLxq6zVwWto3rZ8I5TPELtavglx6cd0Z8uTYMJL3nAx22QuT93GUDHJKG9J0U4DDE9PdsnEfkVAfUUGq+m5yahfsSBo31ZwiHpDSCGZauJDiH4=
---

# 供应链数据看板

## 业务背景

服装供应链涉及面料采购、CMT 生产、品控、入仓多个环节，各环节数据分散在不同表格中，
管理层无法实时掌握生产达成情况，异常问题往往在月度复盘时才被发现。

## 数据来源与规模

- 数据来源：生产记录表、入库记录表、质检记录表
- 数据规模：累计订单约 119.9 万件，覆盖全部生产批次
- 处理方式：Python 通过 API 自动提取并清洗，MySQL 汇总计算

## 分析方法

1. 建立以「批次」为主键的数据对齐模型，打通生产与入库数据
2. 定义核心 KPI：入库达成率、品次率、准时交付率
3. 设置异常阈值，超出范围自动预警

## 可视化

<iframe src="../../assets/charts/supply.html" width="100%" height="520" frameborder="0"></iframe>

## 结论与业务影响

- 入库达成率稳定在 95% 以上，识别出 2 个批次存在交付风险并提前干预
- 品次率异常集中在特定面料供应商，推动采购侧更换供应源
- 月度分析报告取代了原来的人工汇总，单次耗时从 2 天压缩到 10 分钟

## 技术标签

`Python` `MySQL` `Plotly` `自动化报表`
*（内容由AI生成，仅供参考）*
