# 历史人物决策剧场

- ACTIVE_PROJECT: history-crossroads
- 目标：交付用户可直接体验的完整娱乐问答产品，不再停留在选型报告。
- 授权：用户说“你来决定优先做什么吧，我只希望看到可体验的产品”。本轮构建、私有预览发布；不接支付，不推广售卖。
- 允许修改路径：本控制仓 ideas/history-crossroads.md、registry/projects.yaml；业务源码独立放在 Sites 仓库，不进入控制仓。
- 业务源码仓库：https://git.chatgpt-team.site/0ab5af85-dd23-4ea3-9cd0-17b3b128a7ae/appgprj_6adf389afc608191a76263896d518c28.git
- 本地源码：../../sites/history-crossroads
- 阶段：VERIFY；决策 PENDING（商业价值尚未验证）。
- P0：12 道原创情境题、8 种人物风格、选择依据、返回修改、恢复进度、导出结果卡、移动端。
- 验收：答题到结果完整可用；相同答案稳定，不同倾向可产生不同人物；刷新恢复；下载真实图片；手机无横向溢出；不得宣称预测或心理测量准确率。
- P1/P2 后置：收费、双人联测、商城、逐次 AI 报告。
- 复用研究：已核查 SurveyJS MIT 核心库。本体验采用其题目配置和计分能力完成核心答题；结果叙事和视觉为原创。
- 预算：不采购付费 API；运行时模型调用 0；研发 Token、人工时间和平台最终账单未知。先使用现有工具完成单款。
- 商业假设：用户愿意完成并分享有具体解释的娱乐结果。尚无真实完成率、付费或获客数据。
- 计数：handoffs=0，development_reworks=0，full_qa=1。单执行者自检，不冒称独立验证；全量自检结束，不再发起自动评审循环。

## 本轮交付证据

- Sites 业务源码提交：21a2e52b6bfcef788eebe55bd6bcf0f573e7cb48。
- 在线入口：https://szh-history-crossroads.szh0727.chatgpt.site （owner-private）。
- Sites 部署 ID：appgdep_6adf3cc256108191a1fe36c6484dd3e8；2026-10-26T11:43:07Z 回执 succeeded。
- 离线单文件：../../另一种你-可离线体验.html；浏览器已验证进入第一题，无需开发服务器。
- Changed Files：业务仓 dist/{index.html,style.css,content.js,engine.js,app.js,vendor/*}、tests.cjs、README.md、QA.md、.openai/hosting.json；控制仓只改此卡片与登记表。
- Verification：node tests.cjs PASS；8 角色可达且分值机会平衡；两条真实 UI 路线得到张良／徐霞客；返回/恢复/重测与 PNG 解码通过；390px 手机和1280px桌面截图检查。
- Known Issues：未测真实移动设备全部浏览器、收费和营销；自动无障碍扫描装饰图对比度项无法自动判断，已目视检查。没有商业成功结论。
- Next Step：用户直接体验；据具体反馈改题目/结果，不继续增加功能。
