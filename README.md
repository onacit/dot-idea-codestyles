# tour-dot-idea-codestyles

`.idea/codeStyles` 를 공유하기 위한 모듈입니다.

----
## 아직 `.gitmodules` 에 추가되어 있지 않다면

```
$ git submodule add http://bitbucket.wemakeprice.com/scm/nbztb/tour-dot-idea-codestyles.git .idea/codeStyles
```

### `.idea` 디렉토리가 `.gitignore` 에 추가되어 있다면

```
$ git submodule add http://bitbucket.wemakeprice.com/scm/nbztb/tour-dot-idea-codestyles.git .idea/codeStyles
```

----
## 이미 `.gitmodules` 에 추가되어 있다면

```
$ git submodule init && git submodule update
```

### 이미 `.idea/codeStyles` 디렉토리가 존재한다고 에러가 뜨면

```
$ rm -rf .idea/codeStyles
$ git submodule init && git submodule update
```

## IntelliJ IDEA 를 새로 띄워야 적용됩니다.

