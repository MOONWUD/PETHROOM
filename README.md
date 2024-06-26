# Laughing Charlie 🐶 #

        
## Overview 🎁
래핑찰리는 모든 강아지의 일상을 행복하고 웃게 만들겠다는 모토를 가지고 있는 브랜드입니다.      
기존의 웹페이지는 귀여운 캐릭터를 잘 활용하지 못하고 단조롭다는 느낌을 줍니다.        
래핑찰리의 귀여운 캐릭터를 활용한 통통 튀는 디자인을 목표로하고,           
반응형 웹페이지를 구현해 사용자가 편리하게 사용할 수 있도록 퍼블리싱하는 것을         
목표로 선정했습니다.           

       
## Design     
  🍅 Keyword                 
    # 귀여운    
    # 사랑스러운           
    # 통통튀는              
       
  🍅 Color   
     #  00AD4D       
     #  FF2108         
     #  FFD100          
    
           
  🍅 Font  
     - main : Pretendard      
     - title : Poetsen One          
     - point : Bagel Fat One        

          
## Publishing
- GSAP ScrollTrigger를 활용한 다양한 스크롤 이벤트 구현
- SCSS의 @mixin과 @include 활용
- gird와 flex를 활용해 레이아웃 제작 / 제어
- css animation을 활용해 다양한 움직임 적용
- 미디어쿼리를 활용한 반응형 웹페이지 구현

                      
## Probloem & Solution
       💣 모바일 먼저 작업하니 고려해야할 것이 너무 많음, 
          레이아웃이 자꾸 무너지고 제대로 구현하기에 큰 어려움을 겪음.      
          💡 이가 없음 잇몸으로,, 나에게 비교적 쉬운 pc부터 작업,,,        
              보통은 모바일 먼저 작업하지만 아직 나에게 pc가 더 편함.
              
        💣 header에 블러처리를 하고싶으나 filter로 블러처리하면 text까지 블러가 씌워짐     
            💡 새로운 bg영역을 만들어 블러처리했으나 자연스럽지 않음              
            💡 지우고,, 다시 backdrop filter의 blur를 활용하였더니 원하는 느낌을 줄 수 있었음
                     
        💣 main 이미지 위에 텍스트를 고정하기 위해서 
           각각의 감싸는 요소를 만들어 position을 주니 레이아웃이 무너짐     
            💡 grid를 활용해 같은 그리드에 두 요소를 겹쳐 해결!                

        💣 자연스러운 가로 드래그가 이어지지 않음    
            💡 여러 가로 드래그를 시도해 보았으나 실패했음. 
                기존에 내가 구성한 css에 문제가 있을 가능성이 큼              
            💡 아직 완성 시키지 못했고, 시간 나는대로 계속 시도할 예정 !
            💡 클릭 드래그에서 벗어나 스와이퍼를 활용함             

       
        💣 pc에선 스와이퍼 기능이 없는 header를 mo에서 스와이퍼를 넣으니 레이아웃이 깨짐    
            💡 제이쿼리를 활용한 미디어쿼리가 있지만 새로 고침이 필수임 (번거로운과정)           
            💡 스와이퍼 기능을 넣기 위해 pc와 mo header를 따로 만들었음            

        💣 walk와 pogle에 넣은 슬라이드텍스트가,, 크기 제어가 어렵다.
            💡 고정 높이를 줘 크기를 맞췄으니 다양한 사이즈 대응 x                
            💡 해결하기 위해 다른 방법이 필요함 아직 모르겠음   


        💣 맥북 13인치로 봤을 때 자꾸 text nowrap이 활성화되지 않고, 줄바꿈 됨                   
            💡 요소의 전체적인 가로 사이즈를 늘려 텍스트가 딱 맞도록 설정  

        💣 walk와 pogle에 prependTo()와 appendTo()를 사용해서
           버튼이 있을 때만 활성화 되도록 하였으나 움직임이 부드럽지 않음.     
            💡 java의 animate를 이용하여 marginLeft로 밀어내고,            
               자식 요소가 2개까지만 보여줘야함으로 버튼을 2번만 활성화되도록  설정             
            💡 그러나 여전히 부드럽지 못하고 코드를 더할 수록 전체 페이지가 버벅거리면 오류가 남. 
            
                       
## Review 🤸 
                        이번 프로젝트는 작업일지와 변수, 가이드라인을 더욱 꼼꼼하게 작업했다.         
                        새로운 프로젝트에 들어갈 때마다 치밀해지는 나를 발견할 수 있었다.            
                        저번 작업 초기에 고려하지 못한 부분이 나중에           
                        큰 걸림돌이 되었던 것을 기록, 기억해 매번 더 나은 나로 성장하고 있다.  

                        반응형에는 모바일과 태블릿, PC를 다른 디자인으로 
                        디자인하고 구현하는 경우가 있다. 
                        하지만 프로젝트를 기획하는 단계에서 
                        유지보수가 쉽고, 모바일과 PC의 연결이 자연스럽게 구현되길 원했다. 
                        따라서 태블릿을 개별적으로 만들지 않고, PC에서 모바일까지 
                        자연스럽게 연결되는 디자인과 퍼블리싱으로 구현해냈다. 
                                    
                        다만 아쉬운 점은 반응형 웹을 구현할 때 모바일 먼저 작업하지 못한 것이다.            
                        하지만 이번 작업을 통해서 모바일을 먼저 작업하는 이유를 명확하게 알았고,              
                        다음번에는 같은 실수를 반복하지 않을 것이다.               
                                     
                        반응형을 작업하면서 가장 힘들었던 점은          
                        변화하는 사이즈에 대응하여 단위 고려해야한다는 것이다.            
                        세세하게 분기점을 둬 작업할 순 없는 일이다.             
                        유연한 단위를 사용하는 것이 가장 중요하다 느꼈다.              
                                    
                        이번 프로젝트를 마치면서,           
                        강아지는 정말 귀엽다고 느꼈다.            
                        애정을 담아 즐겁게 작업했다.          
                        좋아하는 일을 한다는 것이 얼마나 효율을 높이는지 깨달았다.         
                        설령 좋지 않다하더라도 그 순간만큼은 사랑에 빠진 것처럼             
                        몰입해야겠다 생각했다.           

                
### 240628_금 
  - pc 스와이퍼 이벤트 넣기 완료! (walk, pogle)
  - cutePuppy도 허전한 거 같아 다시 고려해보기               
    -> 강아지가 지나가면 발자국이 생기는 것으로 표현 완료 !!
  - 다양한 모바일 사이즈 구현(고정 크기를 준 요소만 해결하면 됨 !! 그것이 엄청 큰 문제 !
  - nav menu click 영역 확장 

오늘 다 마무리 !!!!

        💥 walk와 pogle에 prependTo()와 appendTo()를 사용해서
           버튼이 있을 때만 활성화 되도록 하였으나 움직임이 부드럽지 않음.     
                      
            💫 java의 animate를 이용하여 marginLeft로 밀어내고,            
               자식 요소가 2개까지만 보여줘야함으로 버튼을 2번만 활성화되도록  설정             
            💫 그러나 여전히 부드럽지 못하고 코드를 더할 수록 전체 페이지가 버벅거리면 오류가 남. 

    
### 240627_목 
  - 햄버거 메뉴 추가 완료 ! 

아자아자 ~ 어색한 부분 다 수정하자 ! 

        💥 맥북 13인치로 봤을 때 자꾸 text nowrap이 활성화되지 않고, 줄바꿈 됨                   
                 
            💫 요소의 전체적인 가로 사이즈를 늘려 텍스트가 딱 맞도록 설정              


### 240626_수
  - 가로 스크롤에만 나타나는 cursor 이벤트 구현 완료 !
  - 가로 스크롤 부드럽게 구현하기 완성 !!!!! (상품 더 추가하기 !!)
  - pc 가로 사이즈 1000px까지는 포용할 수 있도록 부드럽게 만들기 -> 일단은 완료 !
    - margin의 부드러운 움직임 구현
    - 튀어나오는 text요소 글자 크기 줄이기(함수로 제어할 수 있다면 함수로 제어하기)
    - 크기가 고정된 이미지 요소 수정하기
  - 모바일 완성하기 완료 !

아자아자 -! 
오늘 모바일 끝내자 ~
                       
        💥 자연스러운 가로 드래그가 이어지지 않음                    
                 
            💫 클릭 드래그에서 벗어나 스와이퍼를 활용함             
       
        💥 pc에선 스와이퍼 기능이 없는 header를 mo에서 스와이퍼를 넣으니 레이아웃이 깨짐    
                  
            💫 제이쿼리를 활용한 미디어쿼리가 있지만 새로 고침이 필수임 (번거로운과정)           
            💫 스와이퍼 기능을 넣기 위해 pc와 mo header를 따로 만들었음            

        💥 walk와 pogle에 넣은 슬라이드텍스트가,, 크기 제어가 어렵다.
                  
            💫 고정 높이를 줘 크기를 맞췄으니 다양한 사이즈 대응 x                
            💫 해결하기 위해 다른 방법이 필요함 아직 모르겠음              
                           

### 240625_화
  - scss 완성하기 완료 !! (애니메이션까지 완료 ~) 
  - swiper 구현하기 !!!
    - main 완료 !!
    - new 완료 !!
    - mo menu 아직,,,, 
  - java 구현하기  !         
    - textSlide 완료 !
  - pc완성 목표로 화이팅 완료 했음 !!

쉽지 않다. pc는 어찌저찌 완성했지만, 이제 여기서 모바일로 변환하는 과정이 고될 것을 예상.              
또, 스르륵 크기가 작아지는 부분이 엄청나게 버벅거려서 내일 또 봐야함.                   
문제가 많지만 하나하나 해결하면 문제도 아니지.         

        💥 자연스러운 가로 드래그가 이어지지 않음    
                    
            💫 여러 가로 드래그를 시도해 보았으나 실패했음. 
                기존에 내가 구성한 css에 문제가 있을 가능성이 큼              
            💫 아직 완성 시키지 못했고, 시간 나는대로 계속 시도할 예정 !

  
### 240624_월
  - html 설계 완성하기 완료 !         
  - footer 완료 !!!
            
오늘도 어쩐지 버벅거리며 일이 잘 풀리지 않음,,,,,,          
기분이 다운되지만 우울해할 시간이 없고, 우울해 한다고 해결되지 않는다 !               
열심히 해보는 것만이 해결책 ~! 구짭걸 힘을내자             

        💥 header에 블러처리를 하고싶으나 filter로 블러처리하면 text까지 블러가 씌워짐     
                  
            💫 새로운 bg영역을 만들어 블러처리했으나 자연스럽지 않음              
            💫 지우고,, 다시 backdrop filter의 blur를 활용하였더니 원하는 느낌을 줄 수 있었음
                     
        💥 main 이미지 위에 텍스트를 고정하기 위해서 
           각각의 감싸는 요소를 만들어 position을 주니 레이아웃이 무너짐     
                  
            💫 grid를 활용해 같은 그리드에 두 요소를 겹쳐 해결!              
            
    
### 240622_토    
  - 시멘틱 마크업 진행(한 section씩 차근차근 꼼꼼하게 진행)        
  - 미디어 쿼리 범위 고려하기,, + 정리해서 변수 저장 완료        
            
scss랑 사이가 좋은 줄 알았는데 문제가 생겨 처음부터 다시 시작 !        
     
       💥 모바일 먼저 작업하니 고려해야할 것이 너무 많음, 
          레이아웃이 자꾸 무너지고 제대로 구현하기에 큰 어려움을 겪음.      
                  
          💫 이가 없음 잇몸으로,, 나에게 비교적 쉬운 pc부터 작업,,,        
              보통은 모바일 먼저 작업하지만 아직 나에게 pc가 더 편함.
               
### 240621_금
  - 모바일 디자인 완성하기 끝 ~ !
    (집중력 구짭걸)
  - 이미지 정리하기 완료 !! (추가로 필요한 이미지는 그때 그때 편집 저장 ^^;)
  - 시멘틱 마크업 진행(한 section씩 차근차근 꼼꼼하게 진행)
  - og, favicon 설정 완료! 
  - 폰트 설정 완료 !
  - scss 변수 저장하기 완료!
  - header 모바일 작업하기

### 240620_목 
  - text img 만들기
  - 꾸밈 요소 작업하기
  - PC 디자인 완성하기 !
  - 모바일 디자인 시작하기

### 240619_수 
  - PC 디자인 60% 완성

### 240618_화
  새로운 프로젝트 시작 ! 
  - 래퍼런스 사이트 찾기
  - 이미지 정리하기
  - 와이어 프레임 제작하기
