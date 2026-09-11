---
AIGC:
    Label: "1"
    ContentProducer: 001191440300708461136T1XGW3
    ProduceID: 038f982d5cc69ead6143a5e970ea65d2_148ef7bbadb611f18f50525400aeaaa3
    ReservedCode1: zMZcFX6FZqQ74YlAz7VMXMDxvAzwQqG7Dp2sZRHYCGD4n9r3D04JzUeEhifo7IoBBWD+Qzf+xa14/N+O2xDr5/ZtMT8sK4oYkD+Z+e/IOeyfKKNg6mWQtcrKtogQoXs6CuRVfL6B3K1yMfTqDEyU6BA8IgRc4JVJESQ95gdxnTOGo8QvQ7N2LaLO6tE=
    ContentPropagator: 001191440300708461136T1XGW3
    PropagateID: 038f982d5cc69ead6143a5e970ea65d2_148ef7bbadb611f18f50525400aeaaa3
    ReservedCode2: zMZcFX6FZqQ74YlAz7VMXMDxvAzwQqG7Dp2sZRHYCGD4n9r3D04JzUeEhifo7IoBBWD+Qzf+xa14/N+O2xDr5/ZtMT8sK4oYkD+Z+e/IOeyfKKNg6mWQtcrKtogQoXs6CuRVfL6B3K1yMfTqDEyU6BA8IgRc4JVJESQ95gdxnTOGo8QvQ7N2LaLO6tE=
---

# 投放数据看板

## 业务背景

海外广告投放涉及 Facebook、巨量、广点通多个渠道，各渠道后台数据口径不一致，
人工做周报需要反复复制粘贴，且无法实时回答「哪个渠道今天跑亏了」。

## 数据来源与规模

- 数据来源：各投放平台 API、后端消耗数据
- 处理方式：Python 模拟并清洗前后端数据，建立「账户 ID + 日期」对齐模型
- 自动化：函数嵌套实现多维度自动汇总，按渠道动态切换视图

## 分析方法

1. 统一各渠道的消耗与转化口径
2. 构建 ROAS（投入产出比）为核心指标的评价体系
3. 按渠道、按投放人员两个维度拆解绩效

## 可视化

<iframe src="/assets/charts/ad.html" width="100%" height="520" frameborder="0"></iframe>

## 结论与业务影响

- 周报从人工 4 小时缩短到自动生成，且支持按渠道实时切换
- 识别出低效投放组合，调整预算分配后整体 ROAS 有明显改善

## 技术标签

`Python` `MySQL` `Tableau` `数据自动化`
*（内容由AI生成，仅供参考）*
