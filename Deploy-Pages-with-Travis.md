# Travis 自动部署 GitHub Pages

> <https://docs.travis-ci.com/user/deployment/pages/>

## 添加一个 access token

在 GitHub 设置中 <https://github.com/settings/tokens/new> 去添加一个 access token，Travis 自动部署使用到。

## 项目根目录添加 .travis.yml

```yaml
# .travis.yml
language: node_js

node_js:
  - "10"

script:
  - npm run build

deploy:
  provider: pages
  skip-cleanup: true          # 不清除构建过程生成的文件
  github-token: $PAGES_DEPLOY # Travis 对应项目中设置的变量
  keep-history: true          # 保持 commit 记录
  fqdn: example.com           # 自定义域名
  local-dir: dist             # 部署 dist 目录下的文件到 gh-pages 分支
  on:
    branch: master            # 构建 master 分支
```
