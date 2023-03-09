# git hub
작업폴더에서git쓰고 싶으면 <br>
*git init부터 입력 터미널창에<br>
git init 은 레퍼스토리를 하나 생성하는것<br>
파일 현재상태를기록해두려면<br>
*git add 파일명<br>
*git commit -m '커밋내용 '<br>
git add로 기록할파일부터 고르고<br>\
![image](https://user-images.githubusercontent.com/77821108/223604752-45b76dba-65d5-419c-a729-dc4f2a588aef.png)<br>
git add app.txt app2.txt 파일 2개 기록할때<br>
*git add . => 모든 파일은 기록하겠다<br>
*git status =>상태창열기(어떤파일들이<br>
스테이징해놧는지,수정해놧는지 알려주는거)<br>
*git log --all --oneline => commit 내역 조회<br>
commit전에 확인하는것도 좋음<br>
git diff 최근 commitvs현재파일 차이점보여줌<br>
git difftool 커밋아이디 - 현재커밋 vs특정커밋 비교가능<br>
git difftool 커밋아이디 1 커밋아이디2 - 특정커밋 vs특정커밋 비교가능<br>
git graph로 커밋한 기록 볼수있음 이걸 더사용하긴함 git difftool보다<br><br><br>
# branch<br>
branch 기능 이용하면 복사본 만들기 쉬움<br>
![image](https://user-images.githubusercontent.com/77821108/223604900-a186238a-92ae-4ed5-8106-c1b1ecba9eb7.png)<br>
git branch 브랜치명- 브랜치 생성해줌<br>
git switch 브랜치명 - 브랜치로 이동<br>
github.com에서도 브랜치 생성가능<br>
다른 브랜치에서 만든 브랜치 코드를 main브랜치에 합치고 싶을땐<br>
git switch main 으로 이동한후 git merge 합칠 브랜치명<br><br>
같은 파일 같은 줄 수정하면 conflict남<br>
![image](https://user-images.githubusercontent.com/77821108/223605025-6c44ba4b-8458-45e5-a272-265fc8ea78f0.png)<br>
conflict해결법은<br>
1.원하는 코드만 남기고<br>
2.git add<br>
3. git commit<br><br><br>
# git push<br>
git push - u 원격저장소 주소 mian<br>
git push 할때 -u 추가하면 주소 기억하라는 뜻<br>
주소 매일 쓰기 귀찮으니 변수에 주소를저장<br>
git remote add origin(변수명) 주소~~ - 변수명으로 주소를 저장해놓으면 길게 안써도됨<br>
간단하게 git push origin main으로 가능<br><br><br>
# git pull<br>
원격 저장소 복제는
git clone 저장소 주소<br>
팀원 깃헛아이디 등록해놔야 git push 가능<br>
setting에서 collaborators에서 등록<br>
원격 저장소=>로컬저장소<br>
git pull 원격 저장소 주소 브랜치명<br>
변수로 push 할때 지정했으면 그냥 git push 가능<br><br>
*원격저장소 최신내용이 로컬저장소에 있을때만 git push 가능 없으면 pull로 받아야함!!!<br><br>
git pull 할때 브랜치명시가능<br>
특정 브랜치만가져오고싶을때
git pull origin 브랜치명<br>
결론 젤 중요한것!!!!!!!<br>
깃푸시 하기전에 깃 풀부터 해라<br><br>
브랜치 이름 중독 피할려면 사람이름 하거나 브랜치이름 쭉 확인후 알아서 만듬
merge는 거의 github.com에서 함<br>
branch merge 깃허브.com에서도 가능<br>
Pull request가 merge요청임<br>
![image](https://user-images.githubusercontent.com/77821108/223605210-041ac9c7-3b7a-4c80-ae3b-884946ebc5cb.png)<br><br>
![image](https://user-images.githubusercontent.com/77821108/223605227-f6d5594b-0c33-4df0-aa4e-1197e78563eb.png)<br><br>
![image](https://user-images.githubusercontent.com/77821108/223605553-e2644a24-4372-4030-a181-fe73a8d33045.png)


# vue js <br>
wep-app만들때 사용
쉬워서 씀<br>
리액트랑 문법만 다름<br>
html렌더링빠름<br>
업데이트 잘됨 vue3버전 쓸거임<br>
코드는 App,vue에다가 짜면됨<br>
<template>안에는 html 짜고<br>
<script>안에는 js짜고<br>
<style>안에는 css 짬<br>
node.js 16버전 사용 하고잇음<br>
미리보기 띄우고 싶으면 npm run serve<br>

app.vue에 짠 코드를 index.html 에 컴파일 해주는것임<br>
node_modules:프로젝트에 쓴는 라이브러리들<br>
src:소스코드 다 담는곳<br>
public :html파일,기타파일보관<br>
package.json:라이브러리 버전,프로젝트 설정기록<br>
# 데이터 바인딩<br><br>
{{ 데이터 바인딩 }}하는 이유<br>
html 에 하드코딩해놓으면 나중에 변경 어려움<br>
vue의 실시간 자동 렌더링(vue는 신기해서 data를 변경하면 data와 관련된 html에도 실시간으로 반영됨){{}}써야 실시간 자동렌더링 가능<br>
자주 변할것 같은 데이터드은 데이터로 보관하고 html에 {{꽂아넣으셈}}<br>
쇼핑몰 이름은 데이터 바인딩 안해도 됨 왜냐면 애초에 바뀔일이 없으니<br>
데이터는 object자료로 저장<br>
ex)
{자료이름:자료내용}<br>
스크립트 안에 있는 데이터를 html에 꽂아넣고 싶으면
{{ 데이터이름 }} 콧수염기호<br>
html속성도 데이터 바인딩 가능<br>
:속성 = '데이터이름'<br>
ex)<h3 :style='스타일'> 이름</h3><br><br><br>
# vue 반복문<br><br>
<태그 v-for="작명 in 몇회"><br>
 <a v-for="작명 in 3" :key="작명">Home</a> <br>
반복문 쓸때 :key안쓰면 에러남<br>
몇회가 몇번 반복할건지!<br>
vue 반복문 특<br>
array/object 집어넣기 가능<br>
-그럼 자료안의 데이터 갯수만큼 반복됨<br>
-그럼 작명한 변수는 데이터안의 자료가 됨<br>
:key=" " 의 용도<br>
-반복문 쓸때 꼭 써야함<br>
-반복문 돌린 요소를 컴퓨터가 구분하기 위해씀<br>
-변수 작명 2개까지 가능<br>
(a,i) 2개쓰면 가로안에 콤마로 구분<br>
-왼쪽 변수는 array내의 데이터<br>
-오른쪽 변수는 1씩 증가하는 정수<br>


# vue 모달창<br><br><br>
동적인 ui 만드는 법:<br>
ui의 현재 상태를 데이터로 저장해둠(모달창이 지금 어떻게 보여야함?)<br>
데이터에 따라 ui가 어떻게 보일지 작성<br>
v-if="조건식"<br>
은 조건식이 참일때만 html보여줌<br>
셋팅 이렇게 2-step 으로 잘해놓으면 ui켜고 끄기쉽게 가능<br>
실제 상품 데이터를 가져와서 html에 꽂아야함<br><br><br>

# vue 이벤트<br><br><br>
Vue방식은 v-on:click = ""<br>
축약은@click=""<br>
변수++는 변수에 1더해주는 문법<br>
여러가지 이벤트 사용가능<br>
vue에서 함수 만들고 싶으면
methods:{함수(){}} 안에 만드셈<br>
vue에서 함수 만들때 주의 사항<br>
-함수안에서 데이터 쓸땐 this.데이터명<br>
vue개발 팁!!<br>
데이터 어떻게 만들지먼저 생각ㄱㄱ<br>
데이터를 어떻게 만들면내가 편할지 생각<br>
src에 있는거 가져올때 경로는 ./부터


