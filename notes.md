创建基于 typescript 模版的 react 项目

```
npx create-react-app jira --template typescript
```

修改 tsconfig.json, 添加 src 为 baseUrl

安装 prettier

```
npm install --save-dev --save-exact prettier
```

创建 prettier 配置文件

```
echo {}> .prettierrc.json
```

创建.prettierignore 文件，指定无需格式化的文件
https://prettier.io/docs/en/install.html

使用 pre-commit hooks，在代码每次 commit 之前进行格式化
https://prettier.io/docs/en/precommit.html

```
npx mrm lint-staged
```

安装 commitlint，在 git commit 时添加 message 并保证符合规范
https://github.com/conventional-changelog/commitlint

使用 json-server 模拟后端 rest API
https://github.com/typicode/json-server

```
json-server --watch db.json
```
