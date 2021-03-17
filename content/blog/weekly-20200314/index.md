---
title: javascript weekly 2020-03-14
date: "2020-03-14T08:30:00.000Z"
description: "javascript weekly 2020-03-14. 재미난 글이 적어서 VSCode UPdate를 끼워넣음"
tags: ["javascript"]
---

# VSCode 1.43
<a href="https://code.visualstudio.com/updates/v1_43" target="_blank">VSCode 1.43</a>  
+ Search Editor - 서치 에디터(검색 창에서 cmd + enter)에서 검색하면 창 하나에 모든 검색결과와 주변 코드가 나오고, 여기서 수정하면 모든 코드에 반영됩니다.
+ Minimap Sizing Option - 이제 미니맵의 크기를 조절할 수 있습니다.
+ JS/TS Call Hierarchy view - 함수가 호출된 모든 부분을 찾아줍니다.
+ Settings Sync preview - Sync Extenstion을 통해 하던 동기화를 이제 MS에서 지원해줍니다.

# JavaScript: The First 20 Years
<a href="https://zenodo.org/record/3707008#.XmwiXKgzaUk" target="_blank">JavaScript: The First 20 Years</a>  
JS의 창시자 Brendan Eich와 ECMA편집자였던 Allen Wirfs-Brock 의 글입니다.  


# Aborting a Signal: How to Cancel an Asynchronous Task
<a href="https://ckeditor.com/blog/Aborting-a-signal-how-to-cancel-an-asynchronous-task-in-JavaScript/" target="_blank">Aborting a Signal: How to Cancel an Asynchronous Task</a>  
비동기 함수를 취소하는 방법 (abortController의 사용법)을 가르쳐줍니다.  
혹은 카일 심슨의 <a href="https://github.com/getify/CAF" target="_blank">CAF 라이브러리</a>를 활용할 수도 있습니다.


# Slow Code 'Hates Him'.. Optimizing a Web App from 1 to 60 FPS
<a href="https://blog.scottlogic.com/2020/02/17/minesweeper-optimisation.html" target="_blank">지뢰찾기 게임 최적화 하기 후기</a>  
+ store 관리
+ 불필요한 레이아웃 중지 - 웹킷에서 color도 레이아웃에 해당(다른 브라우저는 페인팅) 이 부분을 transparent로 수정
+ 레이어 분할