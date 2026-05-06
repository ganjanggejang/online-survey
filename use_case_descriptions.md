# 팀 코드: `<TODO: 팀 코드 입력>`

# Use Case Descriptions

> **작성 가이드**
> - 각 use case마다 Actor Action / System Response 2열 표로 **step-by-step** 작성
> - ⚠️ 시스템 **내부 동작** (DB 조회, 모듈 호출 등) 작성 금지 (-9점)
> - ✅ Actor가 보고/누르고/입력하는 것 + System이 화면에 보여주는 것만 작성
> - 협업 규칙: `git pull` → 본인 섹션만 수정 → `git push`

---

## 1. 회원 가입

- **Actor**: 사용자
- **담당**: `<서민지>`
- **Brief description**: 사용자가 ID, 비밀번호, 이름, 전화번호, 이메일을 입력하여 회원으로 가입한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.           | 2.              |
| 3.           | 4.              |

**Alternative Courses**
- (필요 시 작성)

---

## 2. 회원 탈퇴

- **Actor**: 회원
- **담당**: `<서민지>`
- **Brief description**: 회원이 본인 계정을 탈퇴하여 모든 이용 권한과 데이터를 삭제한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.           | 2.              |
| 3.           | 4.              |

**Alternative Courses**
- (필요 시 작성)

---

## 3. 로그인

- **Actor**: 회원, 관리자
- **담당**: `<서민지>`
- **Brief description**: 회원 또는 관리자가 ID와 비밀번호를 입력하여 시스템에 로그인한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.           | 2.              |
| 3.           | 4.              |

**Alternative Courses**
- (필요 시 작성)

---

## 4. 설문 등록

- **Actor**: 관리자
- **담당**: `<황보민>`
- **Brief description**: 관리자가 설문 제목, 설명, 문항, 응답 항목, 시작/마감 시각을 입력하여 새 설문을 등록한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1. 관리자가 제목, 설명, 문항, 응답항목, 시작/마감 시각을 입력한다    | 2. 입력 내용을 화면에 표시한다   |
| 3. 관리자가 등록 버튼을 누른다.          | 4.등록 완료 메시지를 표시한다.            |

**Alternative Courses**
- 입력하지 않은 항목이 있는 채로 등록 버튼을 누르면 오류 메시지를 표시한다.

---

## 5. 전체 설문 리스트 조회

- **Actor**: 관리자
- **담당**: `<황보민>`
- **Brief description**: 관리자가 등록된 모든 설문 리스트를 조회한다.

| Actor Action | System Response |
|--------------|-----------------|
|           | 1. 등록된 모든 설문 리스트를 표시한다.         |


**Extensions**
- After step 1, 관리자는 상세 내용 보기를 수행할 수 있다. (Use Case 6)
- After step 1, 관리자는 특정 설문 항목 삭제를 수행할 수 있다. (Use Case 7)

**Alternative Courses**
- 등록된 설문이 없으면 "등록된 설문이 없습니다"를 표시한다.
---

## 6. 상세 내용 보기 (`«extend»` of Use Case 5)

- **Actor**: 관리자
- **담당**: `<황보민>`
- **Brief description**: 관리자가 설문 리스트에서 항목을 선택하여 상세 내용을 팝업으로 본다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.  관리자가 설문 리스트에서 특정 설문 항목을 선택한다.         | 2.  해당 설문의 상세 내용을 팝업 창으로 표시한다.            |
| 3. 관리자가 팝업 창을 닫는다.           | 4.  팝업을 닫고 설문 리스트 화면으로 돌아간다.            |

**Alternative Courses**
- (필요 시 작성)

---

## 7. 특정 설문 항목 삭제 (`«extend»` of Use Case 5)

- **Actor**: 관리자
- **담당**: `<황보민>`
- **Brief description**: 관리자가 설문 리스트에서 특정 항목을 선택하여 삭제한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.  관리자가 설문 리스트에서 삭제할 설문 항목을 선택 후 삭제 버튼을 누른다.          | 2. 해당 설문을 삭제하고 업데이트된 설문 리스트를 보여준다.              |

**Alternative Courses**
- (필요 시 작성)

---

## 8. 설문 검색

- **Actor**: 회원
- **담당**: `<하준수>`
- **Brief description**: 회원이 설문 상태(진행 중/예정/종료)를 선택하고 키워드를 입력하여 설문을 검색한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.           | 2.              |
| 3.           | 4.              |

**Alternative Courses**
- (필요 시 작성)

---

## 9. 검색된 설문 리스트 조회

- **Actor**: 회원
- **담당**: `<하준수>`
- **Brief description**: 회원이 검색 결과로 출력된 설문 리스트를 조회한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.           | 2.              |
| 3.           | 4.              |

**Alternative Courses**
- (필요 시 작성)

---

## 10. 설문 상세정보 보기

- **Actor**: 회원
- **담당**: `<하준수>`
- **Brief description**: 회원이 검색된 설문 리스트에서 특정 설문을 선택하여 새 화면에서 상세 정보를 조회한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.           | 2.              |
| 3.           | 4.              |

**Alternative Courses**
- (필요 시 작성)

---

## 11. 설문 응답

- **Actor**: 회원
- **담당**: `<하준수>`
- **Brief description**: 회원이 진행 중인 설문에 대해 응답을 작성하고 제출한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.           | 2.              |
| 3.           | 4.              |

**Alternative Courses**
- (필요 시 작성)

---

## 12. 통계 정보 조회

- **Actor**: 관리자
- **담당**: `<서민지>`
- **Brief description**: 관리자가 검색 단위(1주일/1개월/1년)를 선택하여 전체 설문 수, 종료된 설문 수, 총 응답 수 통계를 조회한다.

| Actor Action | System Response |
|--------------|-----------------|
| 1.           | 2.              |
| 3.           | 4.              |

**Alternative Courses**
- (필요 시 작성)
