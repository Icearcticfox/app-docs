Артифакты в гитлабе, пример:
```
    artifacts:
        untracked: true
        paths:
            - build/
            - some/**/directories
        exclude:
            - build/dont-include-this-folder/
            - some/**/directories/*.txt
        expire: 1d 
```
[Проблема не работающих exclude](https://gitlab.com/gitlab-org/gitlab/-/issues/15122)
