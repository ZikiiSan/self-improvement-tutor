# Self-Improvement Tutor

本项目基于 Jane Street 的 Agent Skills 中的 Socratic Tutor 改进。导师先用例子讲解，再一次问一个问题，根据你的回答决定下一步。[Jane Street 原版](https://github.com/janestreet/agent_skills/blob/master/socratic-tutor/SKILL.md)

- **用代码验证，让讲解、练习和反馈保持连贯。** 比如讲解折扣回报时，练习沿用例题的奖励序列和折扣系数。导师用代码逐步核对你给出的回报，并用同一个例子解释差异。[查看验证示例](skills/socratic-tutor/references/verifiers.md#worked-example-discounted-return)
- **用一份文档记录学习历程。** 每门课的 `TEACHING_STATE.md` 记录学到哪里、哪些题已独立完成、哪些内容用过提示，以及下次要接着回答的问题。两台电脑都装好 skill 后，只需复制这份文件，就能接着上课。

**在 Codex 中使用**  
在每台设备上，把仓库中的 `skills/socratic-tutor` 文件夹复制到 Codex 的用户 skills 目录（例如 `~/.codex/skills/`），然后在课程目录打开新会话。

1. 开始时说「用 socratic-tutor 教我...」。
2. 离开前说「把我的学习进度和待答问题保存到 `TEACHING_STATE.md`」。
3. 把文件复制到新设备的课程目录，再说「用 socratic-tutor 读取 `TEACHING_STATE.md`，从上次的问题继续」。


---------------------------------------------------------------------------------------------------------------------------------------------
This project builds on Socratic Tutor from Jane Street’s Agent Skills. The tutor works through an example, asks one question at a time, and uses your answer to decide what to teach next. [Original Jane Street skill](https://github.com/janestreet/agent_skills/blob/master/socratic-tutor/SKILL.md)

- **Executable checks keep explanations, exercises, and feedback consistent.** In a lesson on discounted returns, the exercise uses the same rewards and discount factor as the worked example. The tutor checks your return at each step and uses that same episode to explain any discrepancy. [See the verifier example](skills/socratic-tutor/references/verifiers.md#worked-example-discounted-return)
- **One document carries your learning history.** Each course has a `TEACHING_STATE.md` with your current objective, independent work, hints you needed, and the question waiting for you. With the skill installed on both computers, copying that file is enough to resume the lesson.

**Use it in Codex**  
On each device, copy the repository’s `skills/socratic-tutor` folder into your Codex user skills directory (for example, `~/.codex/skills/`). Open a new session in your course folder.

1. Start with “Use socratic-tutor to teach me ...”
2. Before you leave, ask “Save my progress and pending question to `TEACHING_STATE.md`.”
3. Copy the file to the course folder on your other device and ask “Use socratic-tutor to read `TEACHING_STATE.md` and pick up at the pending question.”
