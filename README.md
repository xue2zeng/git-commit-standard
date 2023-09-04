# git commit standard
规范git commit message的模板工具集
## 工具
* git
* npm
* commitlint
* husky
* commitizen
### git创建repo
```shell
create git-commit-standard
cd git-commit-standard
git init
```
### npm
```shell
npm init
```
### commitlint
对`git commit`信息进行检查的工具
```shell
# Install commitlint cli and conventional config
npm i --save-dev @commitlint/{config-conventional,cli}
# Configure commitlint to use conventional config
echo "module.exports = {extends: ['@commitlint/config-conventional']}" > commitlint.config.js
```
### husky
```shell
npx husky-init && npm install
```
### commitizen
一个命令行交互式的 git commit 替代工具
```shell
# First, install the Commitizen CLI tools:
npm install commitizen -g
# initialize project to use the cz-conventional-changelog adapter by typing
commitizen init cz-conventional-changelog --save-dev --save-exact
```