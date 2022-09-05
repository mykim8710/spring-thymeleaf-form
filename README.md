# Spring - Thymeleaf - form Study Project

## Project Spec
- 프로젝트 선택
    - Project: Gradle Project
    - Spring Boot: 2.7.3
    - Language: Java
    - Packaging: Jar
    - Java: 11
- Dependencies: **Spring Web**, **Thymeleaf**, **Lombok**

## 요구사항 정의
- 주제 : 상품을 관리할 수 있는 서비스
- **상품 도메인 모델**
    - 상품 ID, item id
    - 상품명, item name
    - 가격, item price
    - 수량, item quantity
- **상품 관리 기능**
    - 상품 목록 조회
    - 상품 상세 조회
    - 상품 등록
    - 상품 수정
    - 상품 삭제
- 추가기능 : 기존 상품 서비스에 다음 요구사항이 추가
  - 판매 여부
  - 판매 오픈 여부
  - **체크 박스로 선택**할 수 있다.
- 등록 지역
  - 서울, 부산, 제주
  - **체크 박스로 다중 선택**할 수 있다.
- 상품 종류
  - 도서, 식품, 기타
  - **라디오 버튼**으로 하나만 선택할 수 있다.
- 배송 방식
  - 빠른 배송
  - 일반 배송
  - 느린 배송
  - **셀렉트 박스로 하나만 선택**할 수 있다.

## 요청 API 설계
- 상품 **관리 HTTP API URL, Not Rest API**
    - 상품 목록 페이지 :  GET    /form/items
    - 상품 조회 페이지 :  GET    /form/items/{itemId}
    - 상품 등록 페이지 :  GET    /form/items/add
    - 상품 등록      : POST    /form/items/add
    - 상품 수정 페이지 :  GET    /form/items/{itemId}/update
    - 상품 수정      : POST    /form/items/{itemId}/update
    - 상품 삭제      : POST    /form/items/{itemId}/delete

## Spring - form - Thymeleaf 적용
- Spring - thymeleaf 통합
- 입력폼, <input>
- 단일 체크 박스
- 멀티 체크 박스
- 라디오 버튼
- 셀렉트 박스