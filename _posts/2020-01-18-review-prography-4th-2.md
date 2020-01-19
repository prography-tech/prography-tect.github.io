---
layout: post #require
title: "학생개발자의 사이드프로젝트 개발기 2편: 프로토타입 만들기"
author: "dxvinci"
date: 2020-01-18 23:04 # 작성 날짜 등록 
tags: [review, prography] # 원하는 태그 등록 
image: '/assets/posts/dxvinci/review2/7.png'
---


# 3. 1차 마일스톤(5.4)

1차 마일스톤은 그동안 진행한 결과물을 발표하는것이었다. 

## 3.1 제휴 카페 찾기  - round1

주제를 선정한 다음날 유사업체와 제휴하고있는 관악구의 한 카페에서서비스를 직접사용해서 주문을 해보았고 이 업체와 계약한 카페관계자와 인터뷰를 해보며 우리가 다이브해도 괜찮겠다는 확신을 얻었다. 이때까지는 회의록을 쓰던 습관이 남아있어 인터뷰, 기획서들을 참 문서화를 잘 했었다. 이때까지는 아직 문서화가 귀찮다고 생각을 못했던것같다. 

우리는 처음에 서울대학교의 느티나무라는 협동조합을 타겟카페로 삼았다. 외부에 나가기 어려운 서울대학교의 특성상 우리의 서비스가 가장 침투하기 좋은곳이라고 생각했기때문이다. 그렇게 제휴를 맺고자 와이어 프레임까지 만들고 방문을 하였다. 

![2/Untitled.png](/assets/posts/dxvinci/review2/0.png)

그런데 문제가 있었다. 생협에서 운영되는 전사관리 서비스 ERP 시스템에 우리의 어플을 이용한 주문정보를 넣기가 힘들것같다는 답변을 들었다. 즉, 주문이 두군데서 들어오면 일하는사람이 불편해지기 때문이고 이곳은 규모가 꽤 컸기때문에 꼭 주문을 한군데에서 관리를 해야했다. 

![2/Untitled%201.png](/assets/posts/dxvinci/review2/1.png)

더이상 없을것같았던 화상회의가 또 다시 시작되고 있었다... 아직 개발은 시작도 못했는데 말이다. 

*좋은 주제를 정하는건 좋은데, 우리 개발할 수 있는거 맞아?* 

이제 제휴를 맺던 안맺던 개발이 시작되어야했고, 우린 API가 뭔지도 모르는 상황에서 API 기능명세서를 만들어야 했다. 

![2/Untitled%202.png](/assets/posts/dxvinci/review2/2.png)

## 3.2 API 문서를 만들자.

돌아보면 API는 정말 엄청 허술했다. 이제 와서 하는 생각인데 개발을 시작하기전에 API 명세서가 필요한지 모르겠고, 개발을 하면서 API 명세서가 계속 업그레이드 되었어야했는데 우리는 끝까지 이 API 가이드를 사용하지 않았고, 정말 많이 달라졌고 지금도 손님앱에서 서버로 무엇을 주는지, 서버앱에서 점주앱으로 무엇을 주는지 의사소통비용이 계속 발생하고 있다. 1000번 생각해도 이것은 매우 잘못되었지만 해야할게 너무많아 이것을 계속 방치하고 있는 상황이다.🤣

![2/Untitled%203.png](/assets/posts/dxvinci/review2/3.png)

## 3.3 제휴카페를 찾자 - round 2

두번째 타겟으로 설정한 카페는 내가 다니고 있는 학교의 도서관근처에 위치한 커피스퀘어라는 카페이다. 이 카페를 타겟으로 선정한 이유는 사장님이 카페를 차리시기전에 우리학교의 커뮤니티인 고파스를 통해 학생들의 의견을 받았었기에 영하실것이라는 기대가 있었고,  점심시간에 주문이 꽤나 밀리는 편이었기 때문에 니즈도 있을거라고 생각했다.우리가 솔직하게 이야기를 하면 기회를 주시지 않을까?라고 생각했고 떨리는 마음으로 무작정 가보기로 했다.  

![2/Untitled%204.png](/assets/posts/dxvinci/review2/4.png)

*하지만 결과는 대성공! 자 이제 우리 개발은 모르지만 개발 할 수 있는거지..?* 

하지만 뼈개발자출신이 아닌 기획자DNA인 나는 이렇게 까지 힘들게 주제를 정했기에  마케팅이 하고싶어서 지원비를 타야겠다는 생각이 스멀스멀 들고있었다. 

![2/Untitled%205.png](/assets/posts/dxvinci/review2/5.png)

## 3.4 프로토타입과 마크업

1차 마일스톤이었던 5월 4일까지 우리는 sketch로 간단하게 프로토타입을 만들었고 materaiUI를 전부 가져다가 써서 마크업을 만들었다.

![2/Untitled%206.png](/assets/posts/dxvinci/review2/6.png)

*뭐야 materailUI 쓰니까 제법 그럴듯한데?* 

![2/Untitled%207.png](/assets/posts/dxvinci/review2/7.png)

Promise가 무엇인지도 몰랐지만 axios 라이브러리를 보고 난생 처음으로 서버에 있는 메뉴목록을 가져오고 주문을 넣는 서버와의 통신을 성공하고 나니 뭔가 나도 개발자가 될 수 있을것같다는 생각이 들었다. 백앤드를 담당하는 친구와 첫 통신을 하고 방방 뛰었던 기억을 나는 평생 못 잊을것같다. 그렇게 개발이 순조롭게 이어질 줄 알았다.

## 3.5 컴포넌트 구조는 문서화하자

자 이제 여기서 개발 이야기를 해보자. 

설계를 한번도 안해봤던 나는 컴포넌트를 구성할때 재사용성을 고려하지않았다. 확장가능성을 전혀 고려하지 않고 개발을 했기때문이다. 회고 하며 돌아보니 재사용성을 고려할 여유까진 없었던게 자연스러운게 맞는데 컴포넌트간의 흐름에 대해서는 어딘가에 명세가 되어있었어야했던것같다. 상태가 어떻게 흐르는지 적어놓지 않아서 매번 vscode를 왔다갔다 하며 확인했기 떄문이다. 

그리고 구조상 `ScrollableTabsButtonAuto`(주문서)는 `ButtonWithFolderList`(각각의 주문)를 포함할수밖에 없고, `ButtonWithFolderLis`t는 `CustomizedDialogDemo`(모달창)를 포함할수밖에 없어 이런 nested구조가 타당한것이었다. (개발하면서도 계속 잘못되었다고 생각하고 있었다) 

```javascript
    `Menu` = `ScrollableTabsButtonAuto` + `LabelBottomNavigation`(네비게이션)
    
    `ScrollableTabsButtonAuto` > `ButtonWithFolderList`
    
    `ButtonWithFolderList` > `CustomizedDialogDemo`
```

그걸 몰랐던 나는 정말 설계가 초장부터 잘못되어버렸다고 생각했고 , 설계리팩토링을 하지 않았으며 사실 코딩을 길게 하지않았기에 2차마일스톤이 닥치기 전까지는 짠 코드를 들여다 보지도 않았다. 

# **피드백**

**1. 상태 관리에 따라 UI 컴포넌트들의 구조를 그려놓았어야 한다.
2. API 문서는 지속적으로 수정되고 관리돼야 한다.**