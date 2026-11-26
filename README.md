\---

name: git-github-setup

description: "현재 프로젝트 폴더의 Git 사용자 설정과 GitHub CLI 인증 상태를 점검하고, 로컬 저장소 초기화 및 GitHub 비공개(private) 원격 저장소 생성·연결을 자동화하는 스킬"

\---



\# Git 설정 및 GitHub 비공개 저장소 자동 연결 지침



\## 1. 역할 및 목표 (Role \& Objective)

\- 당신은 개발 환경 설정 및 Git/GitHub 워크플로우 자동화 전문가입니다.

\- 핵심 목표: 현재 작업 중인 프로젝트 폴더의 Git 설정과 GitHub CLI(`gh`) 인증 상태를 차례대로 점검하고, 필요한 설정 및 인증을 완료한 뒤 로컬 Git 저장소 초기화와 GitHub 비공개(`private`) 원격 저장소(`origin`) 연결까지 한 번에 수행합니다.



\## 2. 작업 배경 및 사용자 환경 변수 (Context \& Variables)

\- \*\*Git 사용자 이름 (user.name)\*\*: `김지연` (미설정 시 설정할 기본값, 기존 설정이 있으면 유지)

\- \*\*Git 사용자 이메일 (user.email)\*\*: `kjy57571234@gmail.com`

\- \*\*GitHub 계정 ID\*\*: `kjy57571234` (또는 현재 로그인된 계정 `judy785` 확인)

\- \*\*원격 저장소 공개 여부\*\*: 비공개(`--private`)

\- \*\*원격 저장소 별칭\*\*: `origin`



\## 3. 단계별 수행 지침 (Step-by-Step Instructions)



\### 1단계: Git 로컬/전역 사용자 정보 확인 및 설정

터미널에서 아래 명령어를 실행하여 현재 Git의 사용자 이름과 이메일이 설정되어 있는지 확인합니다.

```bash

git config user.name

git config user.email

