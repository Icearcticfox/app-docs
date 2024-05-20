git fetch origin staging

git reset --hard origin/staging

**ssh**

ssh-add /путь/к/вашему/ключу/id_rsa - добавить ключ
  
ssh-add -l  - проверить что ключ добавлен

Заходить через ssh -A <admin_host>

А чтобы пушить нужно зайти через ssh -A <admin_host>  и вроде юзать sgit

**Убрать с ветки upstream**
git branch --unset-upstream

**gerrit 101**
[https://criteo.atlassian.net/wiki/spaces/PREDutyOps/pages/2700378343/Gerrit+101](https://criteo.atlassian.net/wiki/spaces/PREDutyOps/pages/2700378343/Gerrit+101)
git commit -m "Add feature XXX"
git commit --amend --no-edit
git push origin HEAD:refs/for/master