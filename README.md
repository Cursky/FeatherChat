# FeatherChat（羽聊）

![DALL·E 2024-09-25 17.43.37 - A minimalist logo of a small bird perched on a branch with no text, designed with a white background. The bird should be stylized and simple, featurin](https://blog-image-zyt.oss-cn-beijing.aliyuncs.com/undefinedDALL%C2%B7E%202024-09-25%2017.43.37%20-%20A%20minimalist%20logo%20of%20a%20small%20bird%20perched%20on%20a%20branch%20with%20no%20text%2C%20designed%20with%20a%20white%20background.%20The%20bird%20should%20be%20stylized%20and%20simple%2C%20featurin.png)

FeatherChat 是一个开源的鸟类科普聊天网页，结合了目标识别和大语言模型，为用户提供丰富的鸟类知识互动体验。用户可以直接提问获取鸟类知识，也可以上传鸟类图片，系统将识别并提供详尽的科普信息。项目支持多语言（中文、英文）界面，旨在以精美的前后端设计，为用户带来愉悦的使用体验。

## 功能特性

- **智能聊天**：基于 LLM（大语言模型），提供鸟类相关的知识问答。
- **图片识别**：支持用户上传鸟类图片，使用 YOLO v8/v10 模型进行目标识别。
- **RAG 技术**：结合识别结果和知识库，实现检索增强生成，为用户提供准确的科普内容。
- **多语言支持**：界面和交互支持中文和英文。
- **精美设计**：优雅的前端界面，友好的用户体验。

## 项目架构

- **前端（Frontend）**：使用 React.js/Vue.js，支持多语言和响应式设计。
- **后端（Backend）**：基于 FastAPI，提供 API 接口，处理模型调用和业务逻辑。
- **模型（Models）**：
  - **目标识别模型**：YOLO v8/v10，用于鸟类目标检测。
  - **大语言模型**：微调的 LLM，结合 RAG 技术，提供知识回复。
- **知识库（Knowledge Base）**：包含鸟类的科普知识，供 RAG 检索。

## 安装指南

### 前提条件

- Python >= 3.8
- Git

### 克隆项目

```bash
git clone https://github.com/yourusername/FeatherChat.git
cd FeatherChat
