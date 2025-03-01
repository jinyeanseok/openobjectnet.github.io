---
title: "오픈오브젝트 멘토링 수행(프론트개발자)"
last_modified_at: 2022-02-14T18:01:04-04:00
categories: 
  - Mentoring
tags:
  - Mentoring
toc: true
toc_label: "시기별"
author: 감우람   
---

> 멘토링 제도는 신입사원 들어오면 3개월간 멘토를 선정하여, 업무에 잘 적응할수 있도록 하는 제도입니다.   
> 단기별 과제를 통하여 업무에 적응 할 수 있도록 하는것을 목표로 합니다.   
> 첫 단계는 `Javascript를 이용하여 온전한 웹 어플리케이션을 만들고, 해당 어플리케이션이 동작하는 서버환경을 이해하며 직접 서비스까지 진행한다` 입니다.

## 오리엔테이션 - 신입 개발자와 멘토링 시작
>- 우리가 흔히 사용하는 신용/체크 카드의 전산화 과정은 어떻게 될까?
>   - 카드 전산화 과정 및 승인, 전표 매입, 청구, 여신 등의 용어를 설명한다. (by.한수웅 부장님)
>- SI 프로젝트의 진행과정은 어떻게 될까? 
>   - 제안요청 및 작성, 요구사항 수립, 분석/설계, 개발, 테스트, 오픈, 안정화등등 진행과정에 소프트공학에 대해 알아본다. (by.최호남 부장님)
>- SI 프로젝트에 투입이 되면 누구와 어떤일을 할까?
>   - 프로젝트 투입되면 하게되는 대응하는 업무와 카드사 인프라 구조를 설명한다.


## 개발환경  
- IDE : 
  - Visual Studio Code(VScode)
- 실행환경 : 
  - Chrome 웹 브라우저 / Firefox 웹 브라우저
- 소스관리 : 
  - Git (https://github.com). 개인 리파지토리 이용

## 목표
 - VUE(front-end server) 와 NODE(back-end sever) 를 이용하여 로그인과 게시판 기능이 있는 간단한 블로그 스타일 홈페이지를 개발한다.

## 사양
 1. DB(데이터베이스)는 자유롭게 선택
  : mysql, postgree, mongodb, firebase 등
 2. 로그인 시스템은 JWT 토큰 방식 이용
 3. "back-end sever"는 express 서버를 이용  
  -- `기존 express 경험자는 nestjs 를 사용하여 개발(https://nestjs.com/)`
 4. 게시판은 CRUD(create, read, update, delete) 기능 포함
 5. VUE 2 버전으로 개발  
  -- `TYPESCRIPT 적용(class 스타일 적용 안함)`
 6. VUE STORE 기능을 적극 이용
 7. 소스 형상관리는 GITHUB 이용
 8. 완성된 어플리케이션은 자신의 도메인 만들어서 인터넷에서 접근 가능하도록 발행.  
  -- `HTTPS 로 접근 가능하도록 한다`



## 기간
- 언어 적응 및 사양의 내용을 구현. 총 8~10주간 실습 (업무 능력에 따른 시간 소요 변경)
- 마무리 단계에서 작성한 어플리케이션 리뷰-가이드 문서 작성 (보고용)

|   항목                  |   상세                          |   1주  |   2주  |   3주  |   4주  |   5주  |   6주  |   7주  |   8주  |   9주  |   10주  |
|------------------------|--------------------------------|-------|--------|--------|--------|--------|--------|--------|--------|--------|--------|
|   개발환경 세팅           |   장비세팅, IDE, Git             |   O    |        |        |        |        |        |        |        |        |        |
|   언어 습득              |   Modern Javascript 이해        |   O    |   O    |        |        |        |        |        |        |        |        |
|   로그인 시스템 구현       |   Node.js & Express 이해        |        |        |   O    |        |        |        |        |        |        |        |
|                        |  JWT 서비스 구현                 |        |        |        |    O   |        |        |        |        |        |        |
|                        |  데이터베이스 연동                 |        |        |        |        |   O    |        |        |        |        |        |
|   게시판 시스템 구현       |   CRUD API 구현                 |        |        |        |        |        |   O    |        |        |        |        |
|                        |   게시판 화면 구현                |        |        |        |        |        |        |    O   |        |        |        |
|   어플리케이션 발행        |   도메인 등록 및 서비스 구현         |        |        |        |        |        |        |       |   O     |        |        |
|                        |   개발 내용 정리 및 리펙토링        |        |        |        |        |        |        |       |        |     O   |         |
|   리뷰-가이드 문서 작성     |   리뷰-가이드 문서 작성            |        |        |        |        |        |        |       |        |        |     O    |
   

### 1주차 

    - 목표: 업무 적응 및 이해. 개발을 위한 준비
    - 내용: 회사 업무의 기본적인 내용과 개발을 위한 환경을 준비합니다.    

### 2주차 

    - 목표: 최신 문법 Javascript 의 이해
    - 내용: ES6+ 문법을 이해하고 사용합니다.

### 3주차 

    - 목표: Node.js & Express 이해
    - 내용: Javascript 를 이용하여 웹서버를 구현합니다.
    - 선택: 기존 express 경험자는 nestjs 를 사용하여 웹서비스를 구현합니다. 

### 4~5주차 

    - 목표: 로그인 시스템 구현
    - 내용: Backend - JWT를 사용한 토큰 전략과 데이터베이스를 이용한 회원정보 구성을 구현합니다.
    - 내용: Frontend - 토큰을 이용한 로그인 화면을 구현합니다.
    - 선택: Frontend - 회원 가입 페이지를 구현합니다.
    - 선택: TYPESCRIPT 를 적용한다

### 6~7주차 

    - 목표: 게시판 시스템 구현
    - 내용: Backend - CRUD API 를 구현합니다.
    - 내용: Frontend - 게시판 화면을 구현합니다.
    - 선택: TYPESCRIPT 를 적용한다

### 8~9주차 

    - 목표: 어플리케이션 발행
    - 내용: 도메인 구매 및 호스팅 서버에 해당 웹서비스를 전개 / 소스 정리 및 리펙토링
    - 내용: 도메인 구매(개인), 호스팅(개인), 네임서버 설정 및 웹서비스 환경 설정을 진행합니다.
    - 선택: 무료 SSL을 활용하여 HTTPS 로 동작하도록 적용합니다.

### 10주차 

    - 목표: 리뷰-가이드 문서 작성
    - 내용: 동료 개발자 및 부장님, 이사님께 해당 어플리케이션을 설명 및 데모를 진행합니다. (문서 포함)

## 기타
 -
