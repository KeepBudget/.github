# Keep Budget
> Keep Budget은 이사가려고 하는 지역의 `부동산 시세` 및 뉴스를 통해 수집된 `부동산 및 사건사고 정보를 시각화`하여 제공한다.  
> 2인 프로젝트였지만, 웹 서비스 개발은 `내가 담당`

## Service Introduction
저희는 기존 서비스를 이용하면서 다음과 같은 불편함을 느꼈습니다.

> 🙋🏻‍♂️ "부동산 뉴스를 `지역별 세분화`해서 보고 싶어요.😅"<br> 
> 🙋🏻‍♀️ "이사 가려고 하는 지역의 정보를 알고 싶어요."<br>
> 🙋🏻 "안전한 지역으로 이사 가고 싶은데 알 수 있는 방법이 없을까요...😥"<br>

🏘️ Keep Budget을 통해 사용자는
- 희망하는 지역의 부동산 뉴스를 `긍정/중립/부정`으로 나누어 보여주고
- 사건 사고 뉴스를 `워드 클라우드`를 통해 손쉽게 파악 가능하고
- 입력한 값을 통해서 희망하는 지역의 부동산을 추천 받을 수 있습니다.

## ERD
<img width="600" src="https://github.com/user-attachments/assets/8b7af272-7a38-4944-9368-2b9debc7c2c8">

## Project Architecture
<img width="600" src="https://github.com/user-attachments/assets/d90d954b-86af-4b6e-afb4-2f8c0dc56571">

## Main Features
### ⭐️ 부동산 추천 기능
- 희망 지역 & 희망 형태에 해당하는 부동산 데이터를 가져옴
- 가격과 평수를 기반으로 `코사인 유사도`를 계산해 연관성이 높은 순으로 조회

### ⭐️ 사건 사고 뉴스 기능
- 오전 2시에 크롤링 서버가 전일 사건 사고 뉴스를 크롤링해서 저장
- 사용자의 희망 지역에 따라서 뉴스 조회
- 어떤 사건 사고가 일어났는지 `워드 클라우드` 형태로 보여줌

### ⭐️ 부동산 뉴스 기능
- 오전 2시에 크롤링 서버가 부동산 뉴스를 크롤링해서 저장
- 사용자의 희망 지역에 따라서 뉴스 조회
- 해당 지역의 뉴스를 감정 분석을 통해 긍정/부정/중립에 해당하는 뉴스가 어떤 것인지 보여줌

## Screen Configuration
|부동산 실거래가|사건 사고 뉴스|부동산 뉴스|
|:---:|:---:|:---:|
|<img width="150" src="https://github.com/user-attachments/assets/ccbf5ac1-ce6b-49b6-a0e0-4783156a0e28">|<img width="150" src="https://github.com/user-attachments/assets/1cdf1bc5-4562-4bd6-8d31-542309018a84">|<img width="150" src="https://github.com/user-attachments/assets/6f71cc6f-6057-4fca-9004-51ba75efb7f0">|


|지역 수정 기능|로그인 기능|회원가입 기능|
|:---:|:---:|:---:|
|<img width="150" src="https://github.com/user-attachments/assets/8bd57cfe-68b2-431e-806c-6644950931b7">|<img width="150" src="https://github.com/user-attachments/assets/f027f0bc-0335-421e-a675-63e41cd626f3">|<img width="150" src="https://github.com/user-attachments/assets/944e2550-c813-4b58-9407-4228006fc1b8">|
