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
git push origin 브랜치명
결론 젤 중요한것!!!!!!!<br>
깃푸시 하기전에 깃 풀부터 해라<br><br>
브랜치 이름 중독 피할려면 사람이름 하거나 브랜치이름 쭉 확인후 알아서 만듬
merge는 거의 github.com에서 함<br>
branch merge 깃허브.com에서도 가능<br>
Pull request가 merge요청임<br>
![image](https://user-images.githubusercontent.com/77821108/223605210-041ac9c7-3b7a-4c80-ae3b-884946ebc5cb.png)<br><br>
![image](https://user-images.githubusercontent.com/77821108/223605227-f6d5594b-0c33-4df0-aa4e-1197e78563eb.png)<br><br>
![image](https://user-images.githubusercontent.com/77821108/223605553-e2644a24-4372-4030-a181-fe73a8d33045.png)





