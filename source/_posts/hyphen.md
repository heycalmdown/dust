---
title: -(hyphen)
date: 2018-10-07 18:48:04
tags: [shell]
---

유니코드 시대에는 하이픈, 마이너스, N-Dash, M-Dash를 다루는 코드가 따로 있지만(다 비슷하게 생겼다), ASCII 시대에 `-`는 하나뿐이었다.

<!-- more --> 

## cd -

```bash
~/ $ cd haha
~/haha $ cd -
~/ $
```

[manpage](http://man7.org/linux/man-pages/man1/cd.1p.html)에 따르면 `cd`에 따라오는 `-`는 하이픈인데, 처음 `-` 기호를 쓴 사람의 의도는 마이너스였을 거라고 생각한다. 왜냐하면 시간순으로 쌓아온 디렉토리를 하나 뒤로 돌리는 거니까.

## git checkout -

```bash
~/haha master $ git checkout release-1.0
~/haha release-1.0 $ git checkout -
~/haha master $
```

`git checkout`도 같은 논리로 볼 수 있다.

## - on zsh

[zsh](http://www.zsh.org)에서는 `cd`를 생략 가능하다.

```bash
~/ $ haha
~/haha $ -
~/ $ cd a/b/c
~/a/b/c $ ..
~/a/b $ ...
~ $
```

당연히 `..`도 가능하겠고, `...`는 재미로 해보자. zsh에 대해서는 [Oh My Zsh!](https://ohmyz.sh)도 참고

