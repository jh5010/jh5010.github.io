---
layout: post
title: About Git & GitHub
subheading: recording what I studied in Eureka-Project.
author: Jeffrey
categories: jekyll
comments: true
banner:
  video: https://vjs.zencdn.net/v/oceans.mp4
  loop: true
  volume: 0.8
  start_at: 8.5
  image: https://bit.ly/3xTmdUP
  opacity: 0.618
  background: "#000"
  height: "100vh"
  min_height: "38vh"
  heading_style: "font-size: 4.25em; font-weight: bold; text-decoration: underline"
  subheading_style: "color: gold"
tags: Git GitHub Commit Repo
sidebar: []
---

## Git에 대하여

- Git이란: 가장 일반적으로 사용되는 버전 관리 시스템(verison control system)
- 기능: 협업을 쉽게 만들어 여러 사람의 변경 사항을 하나의 소스로 병합할 수 있게끔 함
- 개인이 볼 수 있는 코드를 쓰든, 팀의 일원으로 일하든 유용함

## Git의 특징

- Git이란: 로컬로 실행되는 소프트웨어
- 파일과 파일 기록이 컴퓨터에 저장됨
- 온라인 호스트(예: GitHub 또는 Bitbucket)을 사용하여 파일의 복사본과 해당 수정 기록을 저장 가능
- 변경사항을 업로드하고 다른 개발자의 변경사항을 다운로드할 수 있는 중앙 위치에 있기 때문에 다른 개발자와 더 쉽게 협업 가능
- 자동으로 변경 사항을 병합가능하기 때문에 두 사람이 같은 파일의 다른 부분을 작업하고 나중에 서로의 작업을 잃지 않고 변경사항을 병합 가능

## Git이 코드의 버전 관리를 진행하는 방법

- Git 저장소('Repository', 또는 줄여서 'repo')에는 모든 프로젝트 파일과 전체 수정기록이 포함됨
- 일반 파일 폴더(예: 웹사이트의 루트 폴더)를 가져와서 Git에게 저장소로 만들라고 말함
- 변경 사항을 추적하기 위한 모든 Git 메타데이터가 포함된 .git 하위 폴더가 생성됨
- 이처럼 개인 컴퓨터에 만든 Git Repo를 Local Repository라고 함
- macOS와 같은 유닉스 기반 운영 체제에서는 마침표(.)로 시작하는 파일 및 폴더가 숨겨져 있으므로 숨겨진 파일을 표시하지 않으면 macOS Finder에 .git 폴더가 표시되지 않음.<br>일부 코드 편집기에서 볼 수 있음

## Git에서 새로운 저장소를 만드는 명령어는?

```linux
$ git init
```

## Stage & Commit (어떤 걸 저장할지)
- Commit: 파일 또는 파일 집합에 대해 기록된 각 변경 사항
- 스테이징(Staging): Commit을 진행하기 전에 Git에게 어떤 파일을 commit할지 알려주는 것.<br>__add__ 명령을 통해 진행 가능
- Staging 영역에 파일을 추가한 다음 준비된 파일을 commit한다.

## Remote Repository에 대하여

- Git repo의 복사본을 온라인 위의 호스트(e.g. GitHub, Bitbucket)에 함께 저장하면 변경사항을 업로드하고 다른 개발자의 변경사항을 다운로드할 수 있게 됨
<br> 즉, 여러 개발자 사이 중앙에 위치하므로 다른 개발자와 보다 쉽게 협업 가능
- 원격 Repository를 설정한 후, 파일 및 수정사항 기록을 업로드(__push__)함.
- 다른 사용자가 원격 보고서를 변경한 후 변경 내용을 로컬 보고서로 다운로드(__pull__) 가능.

## Git과 GitHub의 차이점

- 깃은 로컬 파일의 변경사항을 기록하고 해당 파일에 대한 여러 사용자 간의 작업을 조율하기 위한 버전 관리 시스템
- 깃허브는 깃을 클라우드 방식으로 구현된 버전 관리 시스템<br>로컬 파일을 깃허브 클라우드에 __push__(업로드)하여 서로 다른 위치에 있는 여러 사용자가 작업 가능
- 유튜브 노마드 코더 니콜라스의 비유에 따르면, `깃은 '커피'`이고 `깃허브는 '커피샵'`

## GitHub에 대하여

- GitHub란: 원격 저장소를 호스팅하는 `플랫폼`
- 소프트웨어 프로젝트를 저장, 추적 및 협업하는 데 사용됨
<br>이를 통해 개발자는 자신의 코드 파일을 업로드하고 오픈 소스 프로젝트에서 동료 개발자와 협업 가능
- 개발자들이 공개적으로 네트워크 연결, 협업 및 작업 피팅을 할 수 있는 소셜 네트워킹 사이트 역할을 함
- GitHub를 통해 소프트웨어 개발자와 엔지니어는 무료로 클라우드에 __원격 공용 저장소(Remote Public Repository)__를 만들 수 있음.
- GitHub에 Repository를 설정한 후에는 장치로 복사하고 로컬에서 파일을 추가 및 수정한 다음 변경 내용이 대중에게 표시되는 Repository에 변경 내용을 "push" 가능

## GitHub의 장점

1. 협업의 효율화
- Github Repo에는 할 일을 나열하고 게임의 문제를 보곳하고 토론하고 해결한 것으로 표시하기 위한 Issue 섹션도 있음
- GitHub는 몇 명, 수십 명, 심지어 수천 명의 개발자가 다른 사람의 작업을 무시하거나 변경 사항을 추적할 걱정 없이 프로젝트에 원활하게 기여할 수 있는 Cnetralized Workspace를 제공함

2. 쉬운 파일 관리
- GitHub는 Git 위에 그래픽 사용자 인터페이스(GUI) 계층을 추가함
- Git은 자체적으로 Command line(컴퓨터의 Command Line Interface)을 통해 작동함
- 개발자는 명령줄을 사용하는 방법을 알고 있지만 대부분의 경우 명령줄이 파일과 상호 작용하는 가장 효율적인 방법은 아님
- GitHub의 인터페이스는 Git 작업을 수행하고 파일 기록을 볼 수 있는 깨끗하고 사용자 친화적인 수단을 제공함<br>이것은 개발자에게 더 편리하고 Git에 정통한 초보자에게 더 쉽게 접근 가능
- GitHub 사용자는 모든 위치 및 장치엥서 저장소에 액세스하고 레포지토리를 다운로드하고 변경사항을 적용 가능<br>GitHub를 사용하는 것은 하나의 장치나 환경에 제한되지 않음을 의미함

3. 엔지니어들의 SNS