# streamlit_sample

### 👍기간: 2023. 05. 15~ 2023. 05. 17

# EDA

# 탐색적 데이터 분석 EDA

[EDA(Exploratory Data Analysis)](https://www.notion.so/EDA-Exploratory-Data-Analysis-e52fedafce0d4644ac74f8caf710a00b)

[데이터 종류별 시각화](https://www.notion.so/49d5b8fcb94140769bae29b1eda0b925)

# 탐색적 데이터 분석 EDA II

[MATPLOTLIB](https://www.notion.so/MATPLOTLIB-acbbcdb717674565abacf2830b4f887f)

[SEABORN](https://www.notion.so/SEABORN-04f30cd090ee49ae957f1064260d865c)

[PLOTLY](https://www.notion.so/PLOTLY-7b8e980ef3874e8e81fcf81578a66d8a)

# 데이터 EDA

[EDA 실습](https://www.notion.so/EDA-4683b15a452e43889d64fb658fd829f2)

- **JSON**
    
    csv, txt처럼 아예 파일로 써서 파일을 주고받는 방식으로 
    
    <aside>
    💡 JSON (JavaScript Object Notation) 
    텍스트 기반의 가벼운 데이터 형식. 자바스크립트 객체 형식으로 표현된 데이터이기 때문에 웹 클라이언트 측에서 서버측 프로그램으로 쉽게 전달할 수 있다. 이로 인해 웹 활용도가 높다. 표준화, 단순화 , 구조화 되어 있기 때문이다.
    
    </aside>
    
    - 많은 프로그래밍 언어에서 인코딩/디코딩 표준으로 JSON을 제공한다. 파이썬 표준 모듈에도 json이 포함되어 있고, 많은 웹 API들이 JSON형식으로 데이터를 제공한다.
    - MIME 타입은 application/json이며 확장자는 .json이다. 앞쪽 형식에 대한 유형을 알려준다. 웹에서 많이 사용한다. (img, png…)
    
    **JSON의 구조**
    
    - JSON 규칙은 단순하지만 배열 안에 객체를 넣거나 객체 안에 배열을 넣는 방법 등으로 복잡한 데이터를 표현할 수 있다.
    - 실습 : **파이썬으로 JSON 데이터 읽기**
        - JSON의 배열(array)은 파이썬의 리스트(list)와 같으며, JSON의 객체(object)는 파이썬의 딕셔너리(dict)와 같다. → 딕셔너리(dict)는 key : value와 같다.
        
        ```json
        {"@context":"http:\u002F\u002Fschema.org","@type":"ItemList","name":"Things to Do in Sydney","description":"Things to Do in Sydney, Australia: See Tripadvisor's 1,010,579 traveler reviews and photos of Sydney tourist attractions. Find what to do today, this weekend, or in October. We have reviews of the best places to see in Sydney. Visit top-rated & must-see attractions.","ItemListOrder":"http:\u002F\u002Fschema.org\u002FItemListOrderAscending","itemListElement":[{"@type":"ListItem","position":"1","name":"Sydney Opera House","url":"\u002FAttraction_Review-g255060-d257278-Reviews-Sydney_Opera_House-Sydney_New_South_Wales.html"},{"@type":"ListItem","position":"2","name":"Sydney Harbour Bridge","url":"\u002FAttraction_Review-g255060-d257355-Reviews-Sydney_Harbour_Bridge-Sydney_New_South_Wales.html"},{"@type":"ListItem","position":"3","name":"Royal Botanic Garden Sydney","url":"\u002FAttraction_Review-g255060-d257464-Reviews-Royal_Botanic_Garden_Sydney-Sydney_New_South_Wales.html"},{"@type":"ListItem","position":"4","name":"Street Art of Newtown","url":"\u002FAttraction_Review-g8572746-d13743289-Reviews-Street_Art_of_Newtown-Newtown_New_South_Wales.html"},{"@type":"ListItem","position":"5","name":"Drummoyne Oval","url":"\u002FAttraction_Review-g552094-d20154690-Reviews-Drummoyne_Oval-Drummoyne_New_South_Wales.html"},{"@type":"ListItem","position":"6","name":"Marrickville Organic Food and Farmers Markets","url":"\u002FAttraction_Review-g1754380-d3578628-Reviews-Marrickville_Organic_Food_and_Farmers_Markets-Marrickville_New_South_Wales.html"},{"@type":"ListItem","position":"7","name":"Sydney Harbour","url":"\u002FAttraction_Review-g255060-d257842-Reviews-Sydney_Harbour-Sydney_New_South_Wales.html"},{"@type":"ListItem","position":"8","name":"Sauce Brewing Co","url":"\u002FAttraction_Review-g1754380-d12946899-Reviews-Sauce_Brewing_Co-Marrickville_New_South_Wales.html"},{"@type":"ListItem","position":"9","name":"Cockatoo Island","url":"\u002FAttraction_Review-g3668744-d258200-Reviews-Cockatoo_Island-Cockatoo_Island_New_South_Wales.html"},{"@type":"ListItem","position":"10","name":"Birkenhead Point Brand Outlet","url":"\u002FAttraction_Review-g552094-d5485095-Reviews-Birkenhead_Point_Brand_Outlet-Drummoyne_New_South_Wales.html"},{"@type":"ListItem","position":"11","name":"Batch Brewing Co.","url":"\u002FAttraction_Review-g1754380-d7280516-Reviews-Batch_Brewing_Co-Marrickville_New_South_Wales.html"},{"@type":"ListItem","position":"12","name":"Vaucluse House","url":"\u002FAttraction_Review-g13073792-d256728-Reviews-Vaucluse_House-Vaucluse_Woollahra_New_South_Wales.html"},{"@type":"ListItem","position":"13","name":"Elkington Park","url":"\u002FAttraction_Review-g552083-d6487601-Reviews-Elkington_Park-Balmain_New_South_Wales.html"},{"@type":"ListItem","position":"14","name":"South Head Heritage Trail","url":"\u002FAttraction_Review-g552124-d10779778-Reviews-South_Head_Heritage_Trail-Watsons_Bay_Woollahra_New_South_Wales.html"},{"@type":"ListItem","position":"15","name":"Manly Beach","url":"\u002FAttraction_Review-g255060-d257487-Reviews-Manly_Beach-Sydney_New_South_Wales.html"},{"@type":"ListItem","position":"16","name":"Enmore Theatre","url":"\u002FAttraction_Review-g1754380-d7198324-Reviews-Enmore_Theatre-Marrickville_New_South_Wales.html"},{"@type":"ListItem","position":"17","name":"The Bay Run","url":"\u002FAttraction_Review-g552115-d12839844-Reviews-The_Bay_Run-Rozelle_New_South_Wales.html"},{"@type":"ListItem","position":"18","name":"Drummoyne Swimming Centre","url":"\u002FAttraction_Review-g552094-d19857941-Reviews-Drummoyne_Swimming_Centre-Drummoyne_New_South_Wales.html"},{"@type":"ListItem","position":"19","name":"Nielsen Park","url":"\u002FAttraction_Review-g13073792-d258203-Reviews-Nielsen_Park-Vaucluse_Woollahra_New_South_Wales.html"},{"@type":"ListItem","position":"20","name":"Murray Rose Pool","url":"\u002FAttraction_Review-g552126-d556258-Reviews-Murray_Rose_Pool-Woollahra_New_South_Wales.html"},{"@type":"ListItem","position":"21","name":"Darling Harbour","url":"\u002FAttraction_Review-g255060-d257275-Reviews-Darling_Harbour-Sydney_New_South_Wales.html"},{"@type":"ListItem","position":"22","name":"Sydney Ferries","url":"\u002FAttraction_Review-g255060-d1067915-Reviews-Sydney_Ferries-Sydney_New_South_Wales.html"},{"@type":"ListItem","position":"23","name":"Stockade Brew Co Barrel Room","url":"\u002FAttraction_Review-g1754380-d14882303-Reviews-Stockade_Brew_Co_Barrel_Room-Marrickville_New_South_Wales.html"},{"@type":"ListItem","position":"24","name":"Hornby Lighthouse","url":"\u002FAttraction_Review-g552124-d12659944-Reviews-Hornby_Lighthouse-Watsons_Bay_Woollahra_New_South_Wales.html"},{"@type":"ListItem","position":"25","name":"I Have a Dream Mural","url":"\u002FAttraction_Review-g8572746-d8468607-Reviews-I_Have_a_Dream_Mural-Newtown_New_South_Wales.html"},{"@type":"ListItem","position":"26","name":"Birchgrove Park","url":"\u002FAttraction_Review-g552083-d13342979-Reviews-Birchgrove_Park-Balmain_New_South_Wales.html"},{"@type":"ListItem","position":"27","name":"Camperdown Cemetery","url":"\u002FAttraction_Review-g8572746-d8489527-Reviews-Camperdown_Cemetery-Newtown_New_South_Wales.html"},{"@type":"ListItem","position":"28","name":"Sydney Bus Museum","url":"\u002FAttraction_Review-g815420-d12056089-Reviews-Sydney_Bus_Museum-Leichhardt_New_South_Wales.html"},{"@type":"ListItem","position":"29","name":"Tom Uren Walking Trail","url":"\u002FAttraction_Review-g552083-d10663808-Reviews-Tom_Uren_Walking_Trail-Balmain_New_South_Wales.html"},{"@type":"ListItem","position":"30","name":"Chinese Garden of Friendship","url":"\u002FAttraction_Review-g255060-d259700-Reviews-Chinese_Garden_of_Friendship-Sydney_New_South_Wales.html"}]}
        ```
        
        - 결과
            
            ![Untitled](EDA%2027a4040b445a4a14a3ae366992909451/Untitled.png)
            
            [https://jsonformatter.curiousconcept.com/](https://jsonformatter.curiousconcept.com/#)
