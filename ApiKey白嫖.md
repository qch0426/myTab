### 1. Google AI Studio (Gemini API) - *最推荐的稳定白嫖方案*

* **访问地址：** `aistudio.google.com`
* **申请步骤：**
1. 使用你的 Google 账号直接登录。
2. 在左侧导航栏中找到并点击 **"Get API key"**。
3. 点击蓝色的 **"Create API key"** 按钮。
4. 系统会让你选择在一个现有的 Google Cloud 项目中创建，或者点击 **"Create API key in a new project"**（在新建的默认免费项目中创建）。
5. 几秒钟后生成的这串字符就是你的 Key，复制并妥善保存在本地。



### 2. Groq Cloud - *主打极致的响应速度*

* **访问地址：** `console.groq.com`
* **申请步骤：**
1. 打开网页后，建议直接选择使用 GitHub 或 Google 账号快捷授权登录。
2. 进入控制台（Console），在左侧菜单栏点击 **"API Keys"**。
3. 点击右上角的 **"Create API Key"**，给它起个名字（比如 `HN-Summary-Bot`），点击生成并复制。


* *注意：* Groq 的免费层无需绑卡，推理速度极快，但每分钟的并发请求限制相对严格一些。后续我们在写 Python 脚本时，可以稍微加一点延迟（sleep），避免触发风控。



### 3. OpenRouter - *一站式多模型聚合网关*

* **访问地址：** `openrouter.ai`
* **申请步骤：**
1. 访问网站，点击右上角 Sign in，使用账号登录。
2. 进入主页后，点击导航栏的 **"Keys"**。
3. 点击 **"Create Key"**，为其命名并生成。


* *白嫖技巧：* OpenRouter 本身是个代理网关，里面既有收费模型也有免费模型。在后续写代码调用时，只要我们在代码里指定调用那些带有 `:free` 后缀的模型（比如 `meta-llama/llama-3.3-70b-instruct:free` 或者 `google/gemini-2.0-flash-exp:free`），就完全不会产生任何费用。

