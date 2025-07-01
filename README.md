🧑‍💻 중앙 시스템


중앙 시스템은 편의점 내 자산(물품, 장비 등)의 입고, 출고, 재고, 이력 등을 효율적으로 관리하기 위한 자산 관리 시스템입니다.
사용자 역할에 따라 관리자와 일반 직원으로 권한을 분리하고, 자산 등록, 검색, 수정, 삭제, 입출고 처리, 재고 현황 조회 등 핵심 기능을 구현하였습니다.
웹 기반으로 직관적인 UI를 제공하며, 편의점 운영의 효율성을 높이기 위한 목적의 내부 관리 도구입니다.

주)아셀씨앤아이와 연계하여 진행된 기업 맞춤형 개발 프로젝트입니다.

<br/>

## 🛠 기술 스택

| 구분         | 기술 |
|--------------|------|
| Frontend     | React, Vite, chakra-ui |
| Backend      | Spring Boot, WebSocket, JWT |
| Database     | MariaDB |
| Infra/Deploy | AWS EC2, Docker|

<br/>

## ⌛ 개발 기간

- **2025.01 ~ 2025.02 (1달)**

<br/>

## 👥 팀원 소개

| 이름  | 역할 및 담당 업무                                                   | GitHub                                               |
| --- | ------------------------------------------------------------ | ---------------------------------------------------- |
| 민재원 L| •  창고 관리<br>• 로케이션 관리<br>• 물품 입출내역<br>• 재고 실사         | [github.com/Lemonstew](https://github.com/Lemonstew)                                                     |
| 김민경 | •  가맹점 관리<br>• 구매 관리                                  | [github.com/keaimk](https://github.com/keaimk)       |
| 김수민 | •  품목 관리<br>• 공통 코드 관리<br>• 설치 관리                     | [github.com/soomni01](https://github.com/soomni01)   |
| 김용수 | •  인사 관리<br>• 입고 관리                                   | [github.com/Qortn4925](https://github.com/Qortn4925) |
| 김지민 | •  협력 업체 관리<br>• 반품(회수) 관리                            |[github.com/Jin19121](https://github.com/Jin19121)                                                    |
| 윤병관 | •  사업장/부서 관리<br>• 공통 코드 관리<br>• 위치별 재고 현황<br>• 메인 페이지 |  [github.com/y5624711](https://github.com/y5624711)                                                   |

<br/>

## 🧩 서비스 기획 및 설계

### 📌 ERD (Entity Relationship Diagram)

<details>
<p align="center">
  <img src="https://github.com/user-attachments/assets/baeb18fe-31d4-49c5-8748-b77c4477a112" width="600"/>

</p>

</details>


### 📚 메뉴 구조

<details>
<p align="center">
  <img src="https://github.com/user-attachments/assets/ac271cc5-4522-4f4e-8048-2f80ceb14011" width="600"/>

</p>

</details>

### 📚 작업 흐름


<details>
<p align="center">
  <img src="https://github.com/user-attachments/assets/ca9f1984-575d-48fb-84fa-ba89d51ee4a6" width="600"/>

</p>

</details>

## 🖼️ 구현 화면

<details>
<summary>🏠 <strong>로그인/메인 페이지</strong></summary>
  <ul>
    <li>JWT 기반 인증으로 사용자 권한을 구분하여 페이지 접근을 제어합니다.</li>
    <li>사용자 역할(관리자/협력업체)에 따라 노출되는 메뉴가 달라집니다     </li>
  </ul>


<p align="center">
  <img width="48%" alt="KakaoTalk_20250630_200253016" src="https://github.com/user-attachments/assets/9a47c777-25fb-4f89-aa02-9d33f7b39c41" />
  <img width="48%" alt="메인페이지" src="https://github.com/user-attachments/assets/277e7c14-656d-4103-949f-6ad5aa263393" />
</p>

</details>

---

<details>
<summary>➕ <strong>기준정보 관리</strong></summary>
  <ul>
      <li> <strong>기준정보 관리</strong>는 전체 시스템에서 사용하는 주요 마스터 데이터를 관리하는 영역입니다.</li>
      <li>  예: 사업장/창고/협력업체 등의 정보를 등록/수정/삭제할 수 있으며, 등록된 정보는 다른 모듈에서 공통적으로 참조됩니다.</li>
      <li>각 관리 화면은 공통된 UI 패턴을 사용하여 유지보수와 확장성을 고려하였습니다.</li>
  </ul>
<p align="center">
  <img width="48%" alt="사업장관리" src="https://github.com/user-attachments/assets/9bf3fe33-b230-4376-8a51-e3e940d11769" />
  <img width="48%" alt="인사관리" src="https://github.com/user-attachments/assets/3e9a419f-620f-41c7-b093-49e272c82fc1" />
  <img width="48%" alt="가맹점관리" src="https://github.com/user-attachments/assets/c7c2b68f-0338-4c6c-abf0-4e173d55c745" />
  <img width="48%" alt="협력업체 관리" src="https://github.com/user-attachments/assets/c7fe321c-c54d-443c-9897-041acf463900" />
  <img width="48%" alt="품목관리" src="https://github.com/user-attachments/assets/1ec4a883-96fb-4a03-8ecd-3ab4483143ce" />
  <img width="48%" alt="창고관리" src="https://github.com/user-attachments/assets/247eb687-8298-46c2-b7c1-d3308126a3a4" />
  <img width="48%" alt="로케이션관리" src="https://github.com/user-attachments/assets/0ce986d8-4d01-4fd8-a6cd-e8f865bdcce7" />
  <img width="48%" alt="공통코드관리" src="https://github.com/user-attachments/assets/b823ce09-5bc7-4a61-a4ee-70fd0df72006" />
</p>

</details>

---

<details>
<summary>📝 <strong>구매/설치 관리</strong></summary>
  <ul>
     <li><strong>구매 요청부터 설치 완료 및 반품</strong>의 흐름을 관리합니다.</li>
     <li>복잡한 업무 흐름을 효율적으로 관리하기 위해, 상태값을 기반으로 한 단계를 분리하고, 사용자에게 현재 진행 상황을 명확히 보여줍니다.</li>
  </ul>
<p align="center">
  <img width="48%" alt="구매관리" src="https://github.com/user-attachments/assets/6bede5b6-e7d6-44dc-9880-92d9ca1274a1" />
  <img width="48%" alt="입고관리" src="https://github.com/user-attachments/assets/99df9f90-e21f-49b8-9745-1439c34d83f9" />
  <img width="48%" alt="반품회수관리" src="https://github.com/user-attachments/assets/ba78940e-2f11-4c91-8fde-08beef46e667" />
  <img width="48%" alt="설치관리" src="https://github.com/user-attachments/assets/b3502374-3c99-443d-94c6-8dc1b1dc8eba" />
</p>

</details>

---

<details>
<summary>📦 <strong>물류 관리</strong></summary>
  <ul>
    <li>창고 내 물품 입출고 내역, 위치 기반 재고 현황, 재고 실사 기능을 구현하여 <strong>실제 창고 운영에 가까운 환경으로 구현했습니다.</li>
    <li>재고 실사는 바코드 입력 기반으로 빠르게 수량 확인이 가능하도록 구현했습니다.</li>
    <li>로케이션 단위로 나눈 재고현황은 현장 작업자가 직관적으로 재고 분포를 파악하는 데 도움을 줍니다.</li>
  </ul>
<p align="center">
  <img width="48%" alt="물품입출내역" src="https://github.com/user-attachments/assets/f8a9e01e-b964-4ac8-a556-90f87f58077d" />
  <img width="48%" alt="재고실사" src="https://github.com/user-attachments/assets/b1bba59a-ac31-46bc-83f5-78dd0b94d31f" />
  <img width="48%" alt="위치별 재고 현황" src="https://github.com/user-attachments/assets/80e3f7fe-6483-4978-9bce-e983852817bb" />
</p>

</details>
---


