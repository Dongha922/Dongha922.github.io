---
title:  "[Jekyll] 블로그 포스팅하는 방법"
excerpt: "md 파일에 마크다운 문법으로 작성하여 Github 원격 저장소에 업로드 해보자. 에디터는 Visual Studio code 사용! 로컬 서버에서 확인도 해보자. "

categories:
  - Blog
tags:
  - [Blog, jekyll, Github, Git]

toc: true
toc_sticky: true
 
date: 2020-05-25
last_modified_at: 2020-05-25
---
# 프론트엔드(Front-End)

### 😮 프론트엔드 중요한게(역량)

---

1. **미적인 감각(디자인) → Pinterest, Dribble** 
2. 사용자 경험(UX) → 모든 이용자가 쓸 수 있는 페이지를 목표
3. ⭐️ **최신 기술을 빠르게 배워야 한다. → 평생 공부해야해 ㅠㅠ, 구글링, 유명한 블로거 기업들의 소식** 
4. 최고의 친구인 “**벡엔드**”기초를 어느 정도 이해해야 협업이 가능하다!

### 📍 프론트엔드 로드맵

---

[Frontend Developer Roadmap: Learn to become a modern frontend developer](https://roadmap.sh/frontend)

### 🙇‍♂️ 공부 방법

---

**“강의를 보거나 책을 사거나 둘 중 하나”**

강의 : 빨리 공부할 있다, 실무적으로 잘 알려주는게 포인트(제일 쉽게)

책 : 기본적인 개념 탄탄해, 이론적인 책이 훨씬 좋아

→ 강의를 보는게 쉬운 루트!

- **도움이 되는 링크**
    - 인프런(다양한 강좌가 많아서 여기서 마음에 드는 강의로 선택!)
        
        [인프런 - 프로가 되는 온라인 클래스 | 온라인 강의 플랫폼](https://www.inflearn.com/)
        
    - 드림코딩(⭐️ 개인적으로 괜찮은 강좌! 강의 영상이 상세하게 잘 나와있고 내용도 알찬 편!)
        
        [비쥬얼 스튜디오 코드 설치 및 웹개발을 위한 필수 익스텐션 10개 추천 | 프론트엔드 개발자 입문편: HTML, CSS, Javascript](https://www.youtube.com/watch?v=bS9yTI2fC0w)
        
        [Dream Coding](https://academy.dream-coding.com/)
        
        [](https://www.youtube.com/channel/UC_4u-bXaba7yrRz_6x6kb_w)
        
    - 노마드 코더(빠르게 이해하고 싶으면 이거! 공식 문서 기준으로 설명해서 필수 개념은 잘 알려줌!)
        
        [노마드 코더 Nomad Coders](https://www.youtube.com/c/%EB%85%B8%EB%A7%88%EB%93%9C%EC%BD%94%EB%8D%94NomadCoders)
        
        [All Courses - 노마드 코더 Nomad Coders](https://nomadcoders.co/courses)
        
    - 애플코딩(말투가 호불호가 갈리지만…이 유튜브는 약간 미니 요약집으로 생각해서 가볍게 보면 돼!)
        
        [코딩애플](https://www.youtube.com/channel/UCSLrpBAzr-ROVGHQ5EmxnUg)
        
    - 생활코딩(그림체가 단순해서 오히려 시각적인 자료는 부족하지만 이것도 필수 내용만 딱 있음!)
        
        [생활코딩](https://opentutorials.org/course/1)
        

## ✏️ 공부 목표(7월)

---

### 🙋‍♀️ 경희

<aside>
👉 HTML, CSS, JS를 활용한 간단한 **To-Do-List 사이트** 만들기

</aside>

- [ ]  반응형 페이지로 구현되었는지
- [ ]  할 일 추가, 삭제, 수정 기능이 가능한지
- [ ]  적절한 수준의 디자인을 만들었는지
- [ ]  “CSS Hover(참고)”가 적절하게 사용되었는지
- [ ]  현재 해야 할 일, 완료한 일의 갯수가 표시되는지

**별도 미션**

- **개인 GitHub 생성 및 프로젝트 레포에 커밋하여 진행(필수) → 이번 달은 GitHub 사용에 대해서 익숙하기**
- 개인 블로그 또는 우리 노션에 주차별 간단한 회고를 적어줬으면 좋겠음(자유 선택)
- VSCode로 작업하고 반드시 위에 “드림코딩 VSCode Extension 설정” 영상 참고!

### 🙎‍♀️ 동하

<aside>
👉 React + 날씨 API를 활용한 간단한 **일기 예보 사이트** 만들기

</aside>

[기상청_기상특보 조회서비스](https://www.data.go.kr/data/15000415/openapi.do)

- [ ]  컴포넌트별로 잘 구성해서 만들었는지
- [ ]  상태(State) 및 Props 전달이 잘 전달되어 작동하는지
- [ ]  React Hooks를 활용해서 개발했는지
- [ ]  API를 호출하기 위한 Fetch OR Axios 활용을 했는지
- [ ]  반응형 페이지로 구현되었는지
- [ ]  적절한 수준의 디자인으로 만들었는지(어떠한 라이브러리 활용 가능)

**별도 미션**

- **개인 GitHub 생성 및 프로젝트 레포에 커밋하여 진행(필수)**
    
    **→ 이번 달은 GitHub를 경희한테 알려주면서 commit, push, pull, merge, branch 개념에 대해서 정리**
    
- VSCode로 작업하고 반드시 위에 “드림코딩 VSCode Extension 설정” 영상 참고!
- 개인 블로그 또는 우리 노션에 주차별 간단한 회고를 적어줬으면 좋겠음(자유 선택)

### 🤦‍♂️ 상혁(8월까지)

<aside>
👉 Next.js를 활용한 **스터디그룹 사이트** 만들기(졸업작품)

</aside>

- [ ]  Next를 활용하여 적절한 SSR 사이트를 만들었는지
- [ ]  TypeScript를 활용하여 프로젝트를 진행했는지
- [ ]  (Zustand, Redux 중)를 활용하여 상태 관리가 적절했는지
- [ ]  AWS를 활용하여 Serverless 구현 및 배포

## 삭제 금지 ❗❗❗❗

---

[여름방학 일지](https://www.notion.so/0ee489d70e2e4847a904679d4a7f9b6e)
