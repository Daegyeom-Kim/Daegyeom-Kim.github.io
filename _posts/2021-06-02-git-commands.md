---
title: Git Commands
author: Daegyeom Kim
date: 2021-06-02 02:42:00 -0500
categories: [Test, Git]
tags: [tag1, tag2]
---

# Git 명령어 정리

## 생성하기

- git init [project_name/directory] : 새로운 로컬 저장소 생성
- git clone [URL] : 저장소 가져오기

## 살펴보기

- git status : 작업 디렉토리 상태 확인 (파일 정보)
- git diff : 변경된 staged 파일 보기
- git log : 변경 이력 보기

## 브랜치 작업하기

- git branch : 로컬 브랜치 보기
- git branch -av : 로컬과 원격 브랜치 보기
- git checkout <branch> : 브랜치 변경하기
- git branch <new-branch> : 새로운 브랜치 생성하기
- git branch -d <branch> : 브랜치 삭제하기
- git checkout —track <remote/branch> : 원격 브랜치 추적하는 브랜치 만들기
- git branch -u <remote/branch> : 원격 브랜치 추적하기
- git tag <tag-name> : 현재 커밋에 댓글 달기

## 변경하기

- git add [file] : 파일의 변경사항을 다음 commit에 반영하기
- git add . : 모든 변경사항을 다음 commit에 반영하기
- git commit -m "commit massage" : 메시지와 함께 commit하기
- git commit -a : 모든 변경상황을 반영하면서 commit하기
- git commit —amend : 마지막 commit 수정하기(published commit에는 하지 말 것)

## 취소하기

- git reset —hard HEAD : 작업 디렉토리에 모든 변경 버리기
- git revert <commit> : commit 되돌리기

## 동기화하기

- git fetch <remote> : 원격 저장소의 변경사항 가져오기
- git pull <remote> <branch> : 원격 저장소의 변경사항을 가져오고 merge하기
- git pull —rebase : 원격 저장소의 변경사항을 가져오고 rebase하기
- git push : 원격 저장소에 변경사항 발행하기
- git push —tags : 원격 저장소에 태크 발행하기

## 병합하기

- git merge <branch> : 병합하기
- git rebase <branch> : rebase하기

## 변경사항 저장하고 복원하기

- git stash : 임시로 변경사항 저장하기
- git stash pop : 임시 변경사항 복원하기
- git stash list : 임시 변경사항 보기
