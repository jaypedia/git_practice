# Cancling

##### Feb 13, 2022

---

## Cancling git push

- local 내용을 remote에 강제로 덮어쓰기하는 것이니, 주의가 필요하다.
- 되돌아간 commit 이후의 모든 commit 정보는 사라진다.
- 특히 협업을 할 경우 동기화 문제가 생길 수 있으니 팀원과 상의하고 진행하는 것이 좋다.

#### 1. Working directory에서 commit을 되돌린다.

- 가장 최근의 commit을 취소한다.

```
$ git reset HEAD^ // default option : --mixed
```

- 원하는 시점으로 working directory를 되돌린다.

```
// Check commit list
$ git reflog OR $ git log -g
$ git reset HEAD@{number} OR $ git reset [commit id]
```

#### 2. 되돌려진 상태에서 다시 commit을 한다.

```
$ git commit -m "Write Commit Messages"
```

#### 3. 원격 저장소에 강제로 push한다.

```
$ git push origin [branch name] -f
OR
$ git push origin +[branch name]
```

---

### Reference

https://gmlwjd9405.github.io/2018/05/25/git-add-cancle.html
