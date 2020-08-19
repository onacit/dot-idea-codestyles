# tour-dot-idea-codestyles

`.idea/codeStyles` 를 공유하기 위한 모듈입니다.

* 아래 주소에서 `bitbucket`|`stash` 는 현재 module 을 기준으로 바꿔서 사용하세요.
* Protocol 은, 웬만하면, (`ssh://` 가 아닌) `http(s)://` 를 사용하셔야 합니다.

<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
**Table of Contents**

- [tour-dot-idea-codestyles](#tour-dot-idea-codestyles)
    - [아직 `.gitmodules` 에 추가되어 있지 않다면](#아직-gitmodules-에-추가되어-있지-않다면)
    - [이미 `.gitmodules` 에 추가되어 있다면](#이미-gitmodules-에-추가되어-있다면)
    - [IntelliJ IDEA 를 새로 띄워야 적용됩니다.](#intellij-idea-를-새로-띄워야-적용됩니다)

<!-- markdown-toc end -->

----
## 아직 `.gitmodules` 에 추가되어 있지 않다면

특정 모듈에서 처음으로 submodule 을 추가하는 방법입니다.

```
$ git submodule add https://stash.wemakeprice.com/scm/nbzvt/dot-idea-codestyles.git .idea/codeStyles
```

(`.idea` 가 이미 `.gitignore` 파일에 추가되어 있어서) 할 수 없다고 뜨면 `add` 뒤에 `-f` 를 붙이시면 됩니다.

```
$ git submodule add -f https://stash.wemakeprice.com/scm/nbzvt/dot-idea-codestyles.git .idea/codeStyles
```

----
## 이미 `.gitmodules` 에 추가되어 있다면

다른 사람이 submodule 을 추가한 상태라면, pull 을 받았을 때, `.gitmodules` 파일이 신규로 생성된 것을 보실 수 있습니다. 이때는 submodule 을 init/update 만 해 주면 됩니다.

```
$ git submodule init && git submodule update
```

이미 `.idea/codeStyles` 디렉토리가 존재한다고 에러가 뜨면 아래와 같이 해당 디렉토리를 삭제한 후 다시 시도 합니다.

```
$ rm -rf .idea/codeStyles
$ git submodule init && git submodule update
```

## IntelliJ IDEA 를 새로 띄워야 적용됩니다.

해당 프로젝트 창만 새로 띄우면 됩니다.

