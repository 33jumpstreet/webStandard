# WebStandard
- 웹스토리보이님의 강의를 보고 실습하였습니다.   
- 참고) 웹 접근성 연구소 https://www.wah.or.kr:444/ 
---

### 1. 스킵메뉴
- tab을 이용해서 마우스가 아닌 키보드로 화면을 제어하고 메뉴 버튼을 누를 수 있게 하는 기능  

#
### 2. IR효과 
```
- 이미지 대체 텍스트 제공을 위한 css 기법  

/* IR 효과 */
.ir_pm {  /* 의미있는 이미지 텍스트 제공 */
  display: block;
  overflow: hidden;
  font-size: 0;
  line-height: 0;
  text-indent: -9999px;
}
.ir_wa { /* 의미있는 이미지의 텍스트로 이미지가 없어도 대체 텍스트 보여주기 */
  display: block;
  overflow: hidden;
  position: relative;
  z-index: -1;
  width: 100%;
  height: 100%;
}
.ir-su { /* 대체텍스트가 아닌 접근성을 위한 숨긴 텍스트를 제공할 때 */
  overflow: hidden;
  position: absolute;
  width: 0;
  height: 0;
  line-height: 0;
  text-indent: -9999px;
} 
```
> 이외에도 이미지에 텍스트를 설정하고 안보이게 하는 여러 방법이 있다. 아래의 개인 블로그에서 확인 할 수 있다.   
https://moo-you.tistory.com/51
#
### 3. 아이콘 - fontawesome 사이트 이용  
> https://fontawesome.com/v4/icons/  
#
### 4. 어디에서 폰드가 깨지지 않고 보일 수 있도록 구글 웹 폰트 사용 
- 용량이 크기 때문에 다양한 웹 폰트 사용하는 것은 지양하기   
> https://fonts.google.com/ 
#
### 5. 한줄효과 
```
overflow: hidden;
text-overflow: ellipsis;
white-space: nowrap;
```
#
### 6. slick으로 슬라이더 구현
> sclick 사이트 참고   
https://kenwheeler.github.io/slick/
# 
### 7. lightgallery으로 갤러리 슬라이더 구현
> lightgallery 사이트 참고   
https://www.lightgalleryjs.com/docs/getting-started/
