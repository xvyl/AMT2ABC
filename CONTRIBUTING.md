# 贡献指南

感谢您对 AMT2ABC 的关注！我们欢迎任何人以任何形式参与贡献。

## 参与方式

### 1. 提交问题（Issue）

- 使用 Issue 模板创建 **Bug 报告** 或 **功能请求**
- 描述清晰，附上复现步骤（如适用）
- 标签由维护者添加

### 2. 拉取请求（Pull Request）

- 先开 Issue 讨论，避免重复劳动
- Fork 仓库，在 `main` 分支基础上创建新分支
- 遵守代码规范（如有）
- 提交前测试通过
- PR 标题格式：`type(scope): description`（如 `feat(compiler): 支持新目标映射`）
- 等待至少一名维护者审核

### 3. 贡献 AMT 范式

- 在 `data/amt/` 目录下添加 YAML 文件
- 每个 AMT 需包含：ID、名称、因果描述（条件 → 作用 → 结果）、关联的 SECP 指纹
- 通过 PR 提交，由范式评审委员会审核

### 4. 贡献 SECP 指纹模板

- 在 `data/secp/` 目录下添加模板
- 需包含 S/E/C/P 四维的具体定义
- 附上使用说明和示例

### 5. 封装 ABC 模块

- ABC 需独立完成一个业务闭环，不依赖具体设备或字段名
- 提供输入输出 JSON Schema
- 在 `abc-registry/` 下提交元数据，代码可放在独立仓库，通过 Registry 索引

## 开发环境设置

### 克隆仓库

```bash
# GitHub
git clone https://github.com/zylliondata/AMT2ABC.git

# Gitee（国内访问更快）
git clone https://gitee.com/zylliondata/AMT2ABC.git

cd AMT2ABC
```

### 安装依赖

（待补充具体语言环境，如 Python: `pip install -r requirements.txt`）

### 运行测试

（待补充）

## 代码规范

- 遵循 PEP 8（如果使用 Python）
- 注释使用英文或中文均可，但需一致
- 提交信息使用英文，第一行不超过 72 字符

## 行为准则

所有参与者必须遵守 [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)。不遵守者将被禁止参与。

## 获取帮助

- 在 [GitHub Discussions](https://github.com/zylliondata/AMT2ABC/discussions) 提问
- 在 [Gitee Issues](https://gitee.com/zylliondata/AMT2ABC/issues) 留言（中文用户）
- 联系维护者邮箱：info@zylliondata.com

再次感谢您的贡献！
