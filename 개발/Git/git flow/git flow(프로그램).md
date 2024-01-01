![[개발/Git/img/Untitled 8.png|Untitled 8.png]]

> [!info] git-flow cheatsheet  
> created by Daniel Kummer Tweet efficient branching using git-flow by Vincent Driessen translations: English - Castellano - Brazilian Portugues - 繁體中文(Traditional Chinese) - 简体中文(Simplified Chinese) - 日本語 - Türkçe - 한국어(Korean) - Français - Italiano - Nederlands - Русский (Russian) - Deutsch (German) - Català (Catalan) - Română (Romanian) - Ελληνικά (Greek) - Українська (Ukrainian) - Tiếng Việt (Vietnamese) - Polski - العربية - فارسی - Azərbaycanca (Azerbaijani) Bahasa Indonesia Please enable JavaScript to view the comments powered by Disqus.  
> [https://danielkummer.github.io/git-flow-cheatsheet/index.ko_KR.html](https://danielkummer.github.io/git-flow-cheatsheet/index.ko_KR.html)  

참조할 사이트

### `git flow init`

`git flow init` 명령어는 **뒤에 나오는 폴더를 git으로 관리하기 시작**하는 명령어이다 뒤에 아무것도 없으면 **현재 폴더**이다

```Bash
git flow init
```

그럼 사용할 브랜치의 이름을 묻는다==(주로 그냥 enter만 계속 누르면 된다)==

## feature

### **시작**

```Bash
git flow feature start (기능-이름)
```

### **push**

```Bash
git flow feature publish (기능-이름)
```

### **마무리**

```Bash
git flow feature finish (기능-이름)
```

### pull

```Bash
git flow feature pull origin (기능-이름)
```

---

## release

### **시작**

```Bash
git flow release start (버전-이름)
```

### **push**

```Bash
git flow release publish (버전-이름)
```

### **마무리**

```Bash
git flow release finish (버전-이름)
```

### pull

```Bash
git flow release track origin (버전-이름)
```

---

## hotfix

### **시작**

```Bash
git flow hotfix start (버전-이름)
```

### **마무리**

```Bash
git flow hotfix finish (버전-이름)
```