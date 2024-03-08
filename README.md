# clog-ai

使用 AI 自动生成 Commit Log

Generate commit log with AI

## Example

示例可参照本项目的 commit log

You can see the commit log of this project

## Installation

```bash
npm install -g clog-ai
```

## Usage

```bash
clog-ai init
```

then edit config file:

```
{
  "language": "zh or en",
  "datasource": "openai or azure",
  "openai_api_key": "xxxxx",
  "azure_api_key": "xxxxx",
  "azure_deployment_id": "xxxx",
  "azure_base_url": "https://xxxxxxx.openai.azure.com",
  "azure_model": "gpt-3.5-turbo-16k",
  "azure_api_version": "2023-07-01-preview"
}
```

## Run

```bash
git add . # git add files

clog-ai  # generate commit log only

clog-ai --verbose # generate with prompt display
```

![image](https://github.com/aoao-eth/AI-Commit-Log/assets/897401/36b50dc9-5846-424c-a2da-b5149397e1ba)

## Azure api

https://portal.azure.com/

首先免费申请 openai 服务，然后部署 gpt-3.5-turbo-16k 模型，最终将相关的配置写入配置文件

First, apply for openai service for free, then deploy the gpt-3.5-turbo-16k model, and finally write the relevant configuration into the configuration file

## OpenAI api

https://platform.openai.com/api-keys

申请 OpenAI API key，将其写入配置文件中  

Apply for an OpenAI API key and write it into the configuration file.


