# tour-dot-idea-codestyles

`.idea/codeStyles` 를 공유하기 위한 모듈입니다.
아래 주소에서 `bitbucket`|`statsh` 는 현재 module 을 기준으로 바꿔서 사용하세요.

<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
**Table of Contents**

- [tour-dot-idea-codestyles](#tour-dot-idea-codestyles)
    - [아직 `.gitmodules` 에 추가되어 있지 않다면](#아직-gitmodules-에-추가되어-있지-않다면)
        - [`.idea` 디렉토리가 `.gitignore` 에 추가되어 있다면](#idea-디렉토리가-gitignore-에-추가되어-있다면)
    - [이미 `.gitmodules` 에 추가되어 있다면](#이미-gitmodules-에-추가되어-있다면)
        - [이미 `.idea/codeStyles` 디렉토리가 존재한다고 에러가 뜨면](#이미-ideacodestyles-디렉토리가-존재한다고-에러가-뜨면)
    - [IntelliJ IDEA 를 새로 띄워야 적용됩니다.](#intellij-idea-를-새로-띄워야-적용됩니다)

<!-- markdown-toc end -->


----
## 아직 `.gitmodules` 에 추가되어 있지 않다면

```
$ git submodule add http://bitbucket.wemakeprice.com/scm/nbzvt/dot-idea-codestyles.git .idea/codeStyles
```

### `.idea` 디렉토리가 `.gitignore` 에 추가되어 있다면

```
$ git submodule add -f http://bitbucket.wemakeprice.com/scm/nbzvt/dot-idea-codestyles.git .idea/codeStyles
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

