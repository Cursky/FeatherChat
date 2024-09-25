文件架构设计
FEATHERCHAT/
├── frontend/                 # 前端代码（React.js）
│   ├── public/               # 公共资源，如 HTML 模板、favicon 等
│   │   ├── index.html
│   │   └── favicon.ico
│   ├── src/                  # 源码
│   │   ├── components/       # 公共组件
│   │   │   ├── ChatWindow.jsx
│   │   │   ├── ImageUpload.jsx
│   │   │   ├── RecognitionDisplay.jsx
│   │   │   ├── LanguageSwitcher.jsx
│   │   │   └── ...           # 其他组件
│   │   ├── assets/           # 静态资源，如图片、字体
│   │   ├── i18n/             # 国际化配置
│   │   │   ├── index.js      # i18n 初始化
│   │   │   ├── locales/      # 语言文件
│   │   │   │   ├── en.json
│   │   │   │   └── zh.json
│   │   ├── styles/           # 全局和模块化样式
│   │   │   └── index.css
│   │   ├── App.jsx           # 主应用组件
│   │   ├── index.js          # 应用入口
│   │   └── routes.js         # 路由配置（如果需要）
│   ├── package.json
│   ├── package-lock.json
│   └── README.md
├── backend/                  # 后端代码（FastAPI）
│   ├── app/
│   │   ├── main.py           # 应用入口
│   │   ├── api/
│   │   │   ├── routes.py     # 路由定义
│   │   │   └── dependencies.py
│   │   ├── models/           # 数据模型和神经网络模型
│   │   │   ├── yolo_model.py
│   │   │   └── llm_model.py
│   │   ├── services/         # 业务逻辑
│   │   │   ├── recognition_service.py
│   │   │   └── chat_service.py
│   │   ├── utils/            # 工具函数
│   │   │   ├── image_processing.py
│   │   │   └── text_processing.py
│   │   ├── configs/          # 配置文件
│   │   │   └── config.py
│   │   └── __init__.py
│   ├── requirements.txt
│   └── README.md
├── models/                   # 神经网络模型文件
│   ├── yolo/                 # YOLO 模型权重
│   │   └── yolov8_weights.pth
│   └── llm/                  # LLM 模型权重
│       └── llm_weights.bin
├── data/                     # 数据文件
│   ├── knowledge_base/       # 鸟类知识库
│   │   └── bird_knowledge.json
│   └── embeddings/           # 知识库的向量表示
│       └── embeddings.pkl
├── docs/                     # 文档
│   ├── architecture.md       # 架构说明
│   └── api.md                # API 文档
├── scripts/                  # 辅助脚本
│   ├── preprocess_data.py    # 数据预处理脚本
│   └── train_model.py        # 模型训练脚本
├── .gitignore
├── LICENSE
└── README.md
