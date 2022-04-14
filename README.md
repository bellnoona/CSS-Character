# CSS-Character

<br>

## 1. 소개   
- 멋쟁이사자처럼 Front-End School 2기 **천하제일 캐릭터 경진대회** 출품작입니다.
- 🌸벚꽃놀이에 간 어피치🍑의 두근거리는 속마음과 다소 차분한 척하는 겉모습을 표현한 캐릭터입니다. 주변에 흩날리는 벚꽃도 포인트입니다.
- `HTML`, `CSS`만으로 구현하였습니다.
- 해당 페이지에서 배포된 완성본 캐릭터를 볼 수 있습니다. ▶️ <https://bellnoona.github.io/CSS-Character/>

<br>

## 2. 기술
### 2.1 어피치 머리 모양   
  - 생각보다 어피치 머리 모양을 어떻게 구현해야할지 생각해내는 것이 간단하지 않았습니다.   
  먼저 원을 `transform: skewX(9deg)`를 통해서 마름모 모양으로 변형시킵니다. 그리고나서, `transform: rotate(-40deg)`로 회전 시킵니다.   
  그 후, `border-radius`를 통해 둥근 형태를 잡아주어 최종적인 어피치 머리 형태를 만들어주었습니다.     
  
    ( ▶️ 참고 <https://medium.com/@punkyoon/css%EB%A1%9C-%EC%96%B4%ED%94%BC%EC%B9%98-%EA%B7%B8%EB%A6%AC%EA%B8%B0-6ab8da301a4f> )   
    
    ![image](https://user-images.githubusercontent.com/76866502/163362395-cb4c055e-bf1f-4e70-99c2-b018cef49f76.png)

### 2.2 눈동자 애니메이션   
- 눈(eye 클래스)안에 큰 눈동자(twinkle-large 클래스)와 작은 눈동자(twinkle-small)을 두고,    
`@keyframes`를 통해 눈동자가 커졌다 작아졌다를 반복하는 애니메이션 효과를 주었습니다.   

  ![apeach_eyes](https://user-images.githubusercontent.com/76866502/163363275-54adfb8c-0e7a-4bcf-8bf1-d771c0e4a06c.gif)   
  
<br>

## 3. 수정사항   
- 벚꽃이 흩날리는 것을 표현할 때 `HTML`, `CSS` 이외에는 사용하면 안된다고 생각하여 반복작업으로 벚꽃을 표현하였습니다.   
 (div로 원 5개를 만들고 `display: flex;`를 주어서 꽃 한송이당 5개의 원으로 꽃잎을 만들 수 있도록 준비했습니다.   
 `position: absolute;`를 이용해서 원 4개를 가운데로 겹친 다음 `opacity`로 투명도를 높이고 중간에 겹치는 게 비치는 부분은 남은 원 하나를 덧대어 보완했습니다.)    
 
  ![blossom_wind](https://user-images.githubusercontent.com/76866502/163366282-836960e8-dda7-4231-8a5b-0bcf04bb0050.gif)
 
 <br>
 
  ▶️▶️▶️ 추후 수정계획   
 
 1. JavaScript를 이용해서 단순 반복작업으로 작업하던 많은 양의 코드를 짧게 줄일 수 있도록 하겠습니다.   
  or    
 2. `시도` flower.html 같은 식으로 컴포넌트화 해서 똑같은 작업을 반복하던 것을 한번 작업하고 재사용할 수 있도록 바꿔보겠습니다.   
 (원범멘토님 조언을 듣고 시도해보려고 한다. iframe으로 불러오면 될 것 같다고 하시는데 되는지 안되는지는 직접 해봐야 안다.)   
 3. 벚꽃이 오른쪽으로 끊임없이 날아가면서 계속해서 스크롤이 늘어나는 버그를 수정하겠습니다.
 
