# Creator Skills 优化说明（基于 smoke test）

日期：2026-03-11

本次优化依据：`artifacts/skill-tests/*.md` 的实测输出质量与风险点。

## 优化重点

1. **creator-search-intent-radar**
   - 新增信号溯源字段（source/link/captured_at/confidence）
   - 新增 fallback 模式标记（live unavailable 时不伪装成实时趋势）

2. **short-video-hook-lab**
   - 增加 proof-first 证据规则（无验证数据时禁止编造精确数字）
   - 增加 filming complexity 输出字段

3. **creator-deal-ops**
   - 强化 Accept/Negotiate/Decline 决策门槛
   - 新增默认红线（无限返修/权益不清/付款条款缺失）

4. **cross-platform-recut-planner**
   - 增加“首句不可三端相同”与差异化约束
   - 增加 KPI 检查建议

5. **creator-monetization-risk-checker**
   - 明确绿黄红阈值规则
   - 强化禁止“规避平台规则”类输出

6. **ugc-brief-to-script-engine**
   - 增加 brief 缺口假设标记
   - 增加合规交付块（claim safety + mandatory proof shots）

7. **creator-attribution-lite**
   - 增加数据充足性 gate
   - 无真实数据时必须标记 simulation mode
   - 强化“方向性证据，不宣称因果”

8. **batch-content-sprint-os**
   - 增加产能/超载检查逻辑
   - 明确 scope cut 顺序（nice→should→must）

9. **creator-proof-portfolio-builder**
   - 增加证据完整性规则（来源/时间窗/置信度）
   - 明确禁止编造指标

10. **comment-to-content-recycler**
   - 增加去重与近义合并步骤
   - 强化“保留用户原话”与优先级排序

## 验证状态

- 修改后 10 个 skills 全部通过 quick_validate。
