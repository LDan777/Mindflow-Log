Mindflow Log (心流轨迹) 🌊

跨越时区与地点，安放你的情绪、回忆与思维碎片。

作为一个经常在世界各地穿梭的人，跨越时区和地点往往会让时间感变得模糊。内心的感受、情绪和发生的事件交织在一起，很容易让人感到“混乱”。

「心流轨迹」 旨在以一种美观且直观的方式，梳理这些错综复杂的心绪。放弃了可能导致更加混乱的树状图，采用双重视图模式，包容确切的经历与模糊的回忆。

核心功能 ✨

双重视图模式：

🕒 时光轴 (Timeline)：记录带有精确日期的事件，像日记一样梳理线性时间。

🌌 思维碎片 (Fragments)：瀑布流画廊。安放那些“无时间概念”或“模糊回忆”（如：某个夏夜、童年）的情绪、反应和随想。它们在这里自由漂浮。

五大内容维度：

📘 事情 (Event)：客观发生的经历。

🟧 反应 (Reaction)：对人或事的应激反馈。

🌹 情绪 (Emotion)：当下的心境。

🌌 随想 (Thought)：灵光一闪的思考。

🤖 对话/AI (Dialogue)：与人或AI（如 DeepSeek）的深度交流。

AI 对话捷径：选中“对话/AI”分类时，提供一键跳转 DeepSeek 的快捷入口，方便获取灵感并在此归档。

云端同步 (Firebase)：数据实时保存至云端，即使清空浏览器缓存或更换设备，你的记录依然存在。

为什么这么设计？ 💡

当你不知道具体某件事发生在何时，或者只是一段情绪反应时，强制输入日期会让人感到焦虑。
在这里，你可以选择 “模糊回忆” 或 “无时间”，让这些碎片自然地落在右侧的画廊里，而不是被强行塞进日历中。

如何本地运行或部署 🚀

本项目使用 React 和 Tailwind CSS 构建，并依赖 Firebase 进行数据存储。

1. 克隆与安装

git clone [https://github.com/你的用户名/mindflow-log.git](https://github.com/你的用户名/mindflow-log.git)
cd mindflow-log
npm install


2. 配置 Firebase

本项目依赖 Firebase Firestore 来保存数据。你需要在自己的 Firebase 账号中创建一个项目：

前往 Firebase Console 并创建一个新项目。

在项目中添加一个 Web 应用，获取你的 firebaseConfig。

在控制台开启 Firestore Database（建议规则先设置为测试模式）。

在控制台开启 Authentication，并启用 Anonymous（匿名登录） 方式。

在你的项目代码（App.jsx）中，替换 firebaseConfig 部分，并简化数据库路径为 collection(db, 'users', user.uid, 'mindflow_entries')。

3. 运行项目

npm start


或者如果你使用 Vite:

npm run dev


4. 部署到 GitHub Pages

由于本项目是纯前端应用（依靠 Firebase 作为后端），非常适合部署在 GitHub Pages 上。

如果你使用的是 Create React App，可以参考官方文档使用 gh-pages 包进行一键部署。

“时间的流逝在这里变得具体可见，而无序的情绪也找到了安放的坐标。”
