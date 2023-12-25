`config`는 **git**을 **설정**하는 것이다

---

### 이름, 이메일 설정

**이메일**, **이름**을 **설정**한다

**github**의 **이름**과 **이메일**을 적으면 된다.

```Bash
git config --global user.name "seowoo0730"
git config --global user.email "seowoo7718@gmail.com"
```

---

### 설정 확인

**설정**을 **확인**해보려면

```Bash
git config user.name
```

**이름**이 출력 되고

```Bash
git config user.email
```

**이메일**이 출력된다

---

### 설정 확인

모든 설정을 확인할 때는

```Bash
git config --list
```

를 입력하면 된다.

q를 눌러 나올 수 있다.

파일을 직접 보려면

```Bash
git config --global -e
```

그럼 설정 파일이 설정한 에디터로 나온다.

---

## 에디터 설정하기

```Bash
git config --global core.editor "code"
```

또는

```Bash
git config --global core.editor "code --wait"
```

git에서 사용할 에디터를 고르는데 이렇게 하면 vscode가 켜지고 --wait가 붙으면 vscode가 닫히기 전까지는 다른 명령어를 입력할 수 없다.

nano나 vi, vim처럼 명령어로 열거나 사용할 수 있는 에디터를 적을 수도 있다.

---

## 줄바꿈

```Bash
git config --global core.autocrlf input
```

이건 줄바꿈을 할 때 사용이 되는 건데 원래는 window여서 input이 아니라 true로 해야 하지만

주로 wsl을 사용해서 input으로 했다.

---

## git alias

git alias라는 게 있는데

zshrc

와 비슷한데 git에서 명령어들을 줄일 수 있다.

사용방법은

```Bash
git config --global alias.(줄일-명령어) (줄여질-명령어)
```

처럼 해서 바꿀 수 있다.

(앞에 git은 안 붙여도 된다.)

```Bash
git config --global alias.s status
```

명령어 아래에 줄을 긋고 따로 적어 놓겠다.

띄어쓰기가 있다면 ""로 묵는다.

앞에!로 시작하면 git이 아닌 쉘 스크립트로 작동한다

```Bash
git config --global alias.(줄일-명령어) (!줄여질-명령어)
```

git diff 툴 정하기

## git config --global -e로 설정을 열고

```Plain
[diff]
  tool = vscode
[difftool "vscode"]
	cmd = code --diff $LOCAL $REMOTE
```

를 넣으면 된다.

(이건 vscode)

## git merge 툴 정하기

git config --global -e로 설정을 열고

```Plain
[merge]
   tool = vscode
[mergetool "vscode"]
  cmd = code --wait $MERGED
```

를 넣으면 된다.

(이건 vscode)

---

## 한 번에 모든 설정 다하기

### 파일로 하기

```Bash
[alias]
	co = config
	s = status
	i = init
	a = add
	c = commit
	dt = difftool
	mt = mergetool
	l = log --color --graph --decorate --all  --oneline  --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr)%C(bold blue)<%an>%Creset' --abbrev-commit
	ch = checkout
	br = branch
	mer = merge
	ps = push
	pl = pull
	fe = !git fetch && git s
	ac = !git a . && git c
	acm = !git a . && git c -m
	che = cherry-pick
[user]
	name = seowoo0730
	email = seowoo7718@gmail.com
[core]
	editor = code --wait
	autocrlf = input
[diff]
  tool = vscode
[difftool "vscode"]
	cmd = code --diff --wait $LOCAL $REMOTE
[merge]
	tool = kdiff3
[push]
	default = current
[mergetool "kdiff3"]
	path = /mnt/c/Users/이서우/coding/kdiff3/kdiff3.exe
[mergetool]
	keepBackup = false
```

---

```Bash
git co
```