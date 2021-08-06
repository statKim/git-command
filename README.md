# 내가 가끔 쓰는 Git 명령어 모음


## 캐시(Cache) 제거하기
```bash
git rm -r cached .
```


## branch 전환
```bash
git checkout <branch 이름>
```

## Commit 되돌리기
```bash
# 가장 최근의 commit 취소
git reset HEAD^

# 최근 2개의 commit 취소
git reset HEAD~2
```

## 원격저장소 commit 취소하기
```bash
# commit 취소
git reset HEAD^ 

# 다시 commit
git commit -m "commit 메세지"

# 원격저장소에 강제로 push (둘 중 하나 사용)
git push origin <branch 이름> -f
git push origin +<branch 이름>
```
