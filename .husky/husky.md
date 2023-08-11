# 配置husky

## 安装依赖

npm install --save-dev husky

## 初始化husky

npx husky install

## 创建钩子函数

npx husky add .husky/pre-commit "npm run commit"

# 配置commitlint

## 安装依赖

npm install --save-dev @commitlint/cli @commitlint/config-conventional

## 配置文件 commitlint.config.js

module.exports = {
extends: ['@commitlint/config-conventional'],
};

## 添加配置项

"scripts": {
"commitmsg": "commitlint -E HUSKY_GIT_PARAMS"
}

# git

git commit -m "type: subject"
