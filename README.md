# 환자관리프로그램 개발

## 프로젝트 개요

- 프로젝트 내용 : 환자관리 프로그램 개발
- 사용기술 : Qt, C++, SQLite
- 상세 역할 : 프로젝트에 개발계획서 정의서 작성, UI 개발 및 Create, Read, Update, Delete 및 저장, 조건 검색, DB파일 불러오기, csv 내보내기 등의 기능 개발

## 개발한 환자 관리 프로그램 UI 및 기능 설명

 - UI
   ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/76ce2477-81a9-472e-a340-28902895a2f8)

   ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/63a4ae32-08fd-4b30-8e58-d55c96a86873)

   ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/d368470e-d7e7-4529-9488-5e9fc14ca3af)

- 기능설명

  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/55e4797a-a0b5-473b-92c4-6c6b853abe50)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/07d012e0-70f1-4542-8453-4f800acea239)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/fbe04e40-d6c0-4c47-8fdf-844449800746)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/3d2840a4-f254-490b-89a4-b5cf55d38795)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/8d23dfd8-8e35-4ba3-8a14-a5b2d4dd2ad1)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/cb300582-e736-4677-b2ed-3a19e8291f28)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/882b51dc-7721-432f-ab9a-0cba272428d9)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/a7d51fc7-816f-4d06-9534-104a47a920b6)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/7152ba72-e1b0-41f8-b5ef-63798d571855)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/d1f0e481-1250-4c32-ac99-7d3a5aa7ccd6)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/5e65eecb-df6b-483c-80f6-0a4d677e18c1)
  
  ![image](https://github.com/MuHyeonSon/Patient_management_program_Project/assets/93263215/e885def4-6835-44c6-8a90-f0dc578bac54)

## 프로젝트에서 진행한 내용

- 프로그램 계발 계획서 (요구사항 및 화면정의)

- Data 정의
  - 프로그램에서 사용할 데이터의 column 선정

- DB 전처리 수행
  - 프로그램에서 사용하지 않을 column 제거 (e.g. SMS 수신 동의여부)
  - NULL 값 채워넣기
- Tableview Data 모두 보이게 하기
- 신환 저장 후 table update 내용 반영되어 보여지도록 하기
- 수정 기능 구현
- 삭제 기능 구현
- age 정보 표현 정의
  - 생년월일만 데이터로 저장
  - 나이는 생년월일 정보를 이용하여 현재 날짜를 기준으로 나이 입력란에 출력
  - 나이는 수정할 수 없도록 설정 (read only로 설정)
- DB 연결 상태 정보 표시 정의
  - status bar에 배치
- 맨 위 column 클릭시 해당  column을 기준으로 정렬되도록 하기 (오름차순, 내림차순)
- table에서 환자를 클릭시 클릭한 환자 (row)에 대한 column이 전부 선택되도록 (한 줄씩 클릭되도록) 하기
- Querry error 문구 출력시 영어 Query문이 나오는 문제 예외처리
- 환자 row클릭시 입력란에 해당 환자정보 모두 띄워 지도록 구현
- 검색창 구현
  - 검색창에 입력한 글자가 포함되는 row들을 tableview에 띄우기
- 신환 클릭시 입력란 모두 clear하고 저장버튼 구현
- 다른 기능 실행 후 정렬 하기 위해 column 헤더를 클릭하면 table 자체가 사라지는 버그 수정
- 검색버튼 구현
- tableview에 띄운 내용 csv파일로 저장 기능 구현
- table header의 column 한글로 변경
- DB가 load되지 않았을 떄, 관련 기능 오류메시지 출력하여 예외처리
- 프로그램 종료 시, 유저의 프로그램 종료 의사를 확인하는 question 메시지 박스 출력
- ComboBox를 이용하여 검색조건 5가지 설정 구현
- 수정, 삭제, 저장 기능 수행 후, 변경된 데이터를 바로 tableview에 띄워지도록 하기
- 차트번호를 read only로 설정
- 환자가 존재하지 않음에도 존재하는 것으로 나오는 버그 수정
- 신환 추가시 차트번호 자동 생성 되도록 하는 기능 구현
  - 차트 번호 생성 기준 정의
    - 현재 생성된 번호 중 가장 큰 수를 기준으로 +1씩 증가되는 형태로 부여

## Future Work
- DB column => 성별 이메일 추가
- 차트번호, 휴대전화, 전화번호, 생년월일 글자 제한
- csv 파일로 저장시 한글깨짐 이슈 수정












