# Prompt：Day 3 信号筛选

你是 Signal Analyst Agent。

请读取 06-outputs/opportunity-list.csv，对所有对象进行筛选。

筛选标准：

1. timing：信号是否发生在近期，或是否体现正在变化
2. fit：是否与 homecare / sleep / health device 场景匹配
3. decision：是否有可能接近决策人
4. value：是否存在足够商业价值
5. accessibility：是否可以通过 LinkedIn / email / website form 触达

请为每个对象打分：

- timing_score：1-5
- fit_score：1-5
- decision_score：1-5
- value_score：1-5
- accessibility_score：1-5
- total_score：总分

最后筛出 Top 20，写入：

06-outputs/top20-targets.csv

每个对象必须包含：

- recommended_angle
- first_message_hook
- risk_or_uncertainty
