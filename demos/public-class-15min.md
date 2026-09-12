# 《当AI成为运营伙伴》

## Seedance 2.5 AI商业导演案例

这是公开课的 15 分钟可展示 Demo。展示目标不是“写一段 Prompt”，而是让观众看到同一个商业需求如何经过导演分析、分镜、摄影指导、Prompt 编译和质量检查，变成可执行的视频生产方案。

## Demo准备

```text
Skill: seedance-cinematic-director
Model: Seedance 2.5
Duration: 30 seconds
Aspect ratio: 16:9
Reference set: character identity, office scene, training-hall wide/left/right/stage/audience, style reference
```

现场可将本文件与 `examples/GEO-growth-journey.md` 并排展示：前者是演示讲稿，后者是案例素材和最终 Prompt。

## 1. 提出需求｜30秒

展示输入：

```text
我要制作一个GEO运营训练营宣传片。

目标：让企业负责人理解AI正在改变运营方式。
风格：苹果发布会级、高端商业纪录片。
```

讲解重点：普通 Prompt 只描述“做一个公司视频”；导演 Skill 先识别商业目标、受众和传播目的。

## 2. AI导演分析｜2分钟

展示输出：

```text
创意定位：从人工运营时代进入AI运营时代。
核心冲突：过去依赖经验试错，未来依靠AI能力系统。
情绪曲线：困惑 → 学习 → 突破 → 自信。
商业记忆点：AI不是替代运营者，而是成为运营伙伴。
视觉策略：冷色办公室的停滞感，经过蓝紫训练环境，进入暖色高效工作状态。
```

讲解重点：主题、冲突、情绪和品牌记忆点先于镜头词汇。

## 3. 自动生成30秒结构｜3分钟

展示输出：

```yaml
SHOT 01:
  time: 0-8s
  scene: 深夜办公室
  action: 运营人员面对停滞数据和散乱的GEO资料
  meaning: 人工运营时代的瓶颈

SHOT 02:
  time: 8-20s
  scene: AI训练环境
  action: 进入训练会场，学习GEO方法论，使用AI Skill拆解问题
  meaning: 从困惑到方法

SHOT 03:
  time: 20-30s
  scene: 回到工作场景
  action: 运营人员与团队用AI辅助完成清晰运营方案
  meaning: 新时代工作方式和品牌价值
```

讲解重点：每个段落同时有时间、空间、动作和商业含义，避免只有“画面很高级”。

## 4. 摄影指导生成｜3分钟

展示输出：

```text
SHOT 01
Camera: 40mm ARRI-style cinematic camera, slow dolly in, shallow depth of field, restrained rack focus from stalled data to the operator's eyes.
Lighting: computer blue light, cold white ceiling light, low saturation, controlled pressure.

SHOT 02
Camera: 85mm portrait compression for the learning beat, rack focus from the operator to the far stage screen, then a measured track from the fixed aisle.
Lighting: blue-purple AI stage light with a motivated warm key from the presentation area.

SHOT 03
Camera: 35mm commercial documentary coverage, restrained arc move around the team, stable final framing for the brand memory point.
Lighting: warm practical work light, natural skin tone, visible feeling of capability and growth.
```

讲解重点：镜头不是堆砌“电影感”，而是用焦段、运动、焦点和光线解释情绪变化。

## 5. Seedance Prompt输出｜5分钟

展示最终 Prompt：

```text
Project: 当AI成为运营伙伴
Duration: 30 seconds
Aspect Ratio: 16:9
Visual Style: premium commercial documentary, restrained Apple-launch-level precision, realistic live action.

Business Goal: show enterprise decision-makers that AI changes the operating method and becomes a practical operating partner.

Character: 28-year-old Asian male GEO operator, consistent face, age, hairstyle, body proportions, dark practical wardrobe, and notebook across every shot. Preserve identity; allow only shot-specific gaze, expression, hand, posture, and weight changes.

Reference Roles: Image 1 controls character identity only; Image 2 controls the office layout only; Images 3-7 are wide, left, right, stage, and audience views of one training hall; Image 8 controls color and atmosphere only. Do not inherit background or lighting from the identity image, and do not let the style image change face or venue geometry.

Scene: one coherent office and one coherent AI training hall. In the hall, the entrance remains camera-left, the aisle camera-right, the stage screen at the far end, and the audience faces the stage.

Timeline: 0-8s, cold blue late-night office, stalled data and scattered GEO notes, operator scans the screen and exhales, slow 40mm dolly in with shallow depth of field. 8-20s, motivated light bridge into the same fixed training hall, enter from camera-left, track along the camera-right aisle, facilitator points to the far screen, operator's eyes follow first and the body turns with natural weight transfer, blue-purple stage light with a warm key. 20-30s, return to a warm work setting, team reviews a clear plan, operator presents with credible eye-lines and hand contact, restrained 35mm arc move, hold a stable readable brand end state.

Sound: office room tone, restrained keyboard and ventilation, training-hall ambience, subtle confident voice, no distracting music and no excessive on-screen text.

Continuity Rules: same person, same wardrobe, same notebook; preserve venue landmarks, entrance direction, stage position, screen direction, seating order, and realistic human causality across cuts. Use one dominant camera movement per shot.

Negative Prompt: face change, age change, hairstyle change, wardrobe change, duplicate people, spatial drift, reversed screen direction, moved stage, unreadable logo, excessive text, extra limbs, broken hands, impossible physics, abrupt camera jumps, unmotivated lighting changes.

End State: warm, stable commercial frame with the operator and team facing the clear plan, brand mark readable, no new objects entering the frame.
```

讲解重点：最终 Prompt 同时包含商业目标、参考图职责、人物锁定、空间记忆、时间轴、摄影、灯光、声音、连续性和禁止项。

## 6. 生成后质量检查｜2分钟

展示检查结果：

```text
人物：✅ 同脸  ✅ 同服装  ✅ 无年龄变化  ✅ 动作与身份分离
空间：✅ 办公室逻辑稳定  ✅ 会场入口/舞台/座位/屏幕方向稳定
商业：✅ 有开始-转化-结果  ✅ 情绪完整  ✅ 有品牌价值
Seedance：✅ 避免过多文字  ✅ 动作在时长内  ✅ 无明显不可能物理
结论：PASS，允许进入生成或小范围镜头迭代。
```

## 最后一页：定位升维

```text
Prompt时代
告诉AI做什么
        ↓
Skill时代
教AI如何像专业团队一样工作
        ↓
Agent时代
AI成为你的数字团队
```

## 企业增长闭环

```text
GEO Skill
让AI理解企业：品牌、业务、用户和增长机会
        ↓
Seedance Skill
让AI表达企业：商业故事、人物、镜头和品牌视频
        ↓
Content Skill
让AI传播企业：文章、短视频、社媒和转化内容
```

演讲落点：`matutuai.cn` 不是 Skill 收藏库，而是企业 AI 能力资产平台；GEO 负责理解，Seedance 负责表达，Content 负责传播。
