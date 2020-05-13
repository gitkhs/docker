# 깃허브 기본 기능

### git clone

### fetch 와 pull

원격 저장소의 데이터를 로컬로 가져 온다.
`pull`은 데이터를 가져온 후 로컬과 병합,
`fetch`는 데이터만 가져 오고 로컬과 병합하지 않는다.

### checkout

모든 작업은 원격 저장소를 기준으로 한다.

## 브랜치
```bash
# 저장소 받아오기
git clone <url>

# 저장소 변경사항 받아오기
# pull은 원격에서 받아와 로컬과 머지 하며 fetch는 머지 하지 않는다
git fetch

# 브랜치 목록 조회
# -r 옵션으로 원격 저장소의 브랜치를 조회 한다.
git branch

# 브랜치 선택
# 체크아웃시 원격저장소에 동일한 이름의 브랜치가 존재 하면
# 로컬저장소의 브랜치를 생성 후 선택 한다.
git checkout <branch>

# 브랜치 병합
# 해당 브랜치의 내용과 병합한다.
git merge <branch>

# 원격 저장소에 전송
# 
git push <remote> <branch>
```