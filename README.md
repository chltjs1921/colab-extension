# colab-extension
vs code서 colab과 cc extension을 연결해서 사용할 수 있나 테스트

colab서 claude code를 써보고 싶었음. 
로컬의 vs code를 오작교처럼 사용해서 저 둘을 연동할 수 있는지 테스트해봄

1/11 상황
- colab extension으로 구동시킨 노트북을 claude code extension으로 읽게 시킴 >> 읽기 성공

1/18 상황
-파일 업로드, 마운트만 된다면 코랩과 claude code를 연동할 수 있다는 것을 확인. sample data로 간단한 mlp 만들기 성공. 

1/24~1/25 시도해볼 거
- 굳이 마운트일 필요는 없다 그러므로 어떻게든 colab에 연결된 노트북이 파일을 읽게 만들어야 한다.
- 다른 일로 대전을 갔다와서 이 날들은 패스

1/29
- https://github.com/googlecolab/colab-vscode/wiki/User-Guide
- 이제는 파일 올리기가 되는건가

2/8
- 마운트 성공. 단, 2가지 문제 존재
    1. 파일의 경로를 제대로 입력해주어야 함. 옆 사이드에 드라이브 정보가 보이지 않음. 따라서 웹상에서 직접 경로를 추적해야 함
    2. claude code는 노트북에 코드 입력이 끝. 실행은 온전히 나의 몫. 만일 문제 해결해야 되는 상황이라면 claude code도 직접적인 분석이 힘들 수 있다.
