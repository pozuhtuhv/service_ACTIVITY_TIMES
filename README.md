## Setting up Pinmycommit (ver Python, GitActions)

## 0. 준비사항
- (매우중요) `Repo를 Fork`를 진행한 후 `Fork된 Repo`에서 진행

### 1. Generate Personal Access Token
1. GitHub에서 [Personal Access Token 생성 페이지](https://github.com/settings/tokens)로 이동합니다.
2. `New personal access token`을 클릭합니다.
3. `repo`와 `gists` 권한을 체크한 후, 만료 기간(Expiration)을 설정합니다.
4. `Generate token`을 클릭하여 토큰을 생성합니다.
5. 생성된 토큰을 복사합니다.

### 2. Create a Gist
1. [Gist](https://gist.github.com/) 페이지로 이동하여 새로운 Gist를 생성합니다.
2. `Name` 필드에 `Commit_Times`라고 입력합니다. (내용은 없어도 됨)
3. `Create public gist`를 클릭하여 Gist를 생성합니다. (`secret gist`가 아닌 `public gist`로 생성)
4. 생성된 Gist URL의 ID를 복사합니다.
   - 예시: `https://gist.github.com/yourname/*************` (`*************`를 복사).

### 3. Add Secrets to Your Repository
1. 레포지토리의 `Settings` -> `Secrets and variables` -> `Actions`로 이동합니다.
2. `New repository secret`을 클릭합니다.
3. `Name` 필드에 `ACCESS_TOKEN`을 입력하고, 앞서 복사한 `Personal Access Token`을 붙여넣습니다.
4. `Add secret`을 클릭하여 저장합니다.
5. 동일한 방법으로, `Name` 필드에 `GIST_ID`를 입력하고 생성한 `Gist의 ID`를 붙여넣습니다.
6. `Add secret`을 클릭하여 저장합니다.
7. 동일한 방법으로, `Name` 필드에 `USER_NAME`을 입력하고 `자신의 GitHub 사용자 이름`을 붙여넣습니다.
8. `Add secret`을 클릭하여 저장합니다.

### 4. 참고 문서
- [Commit 검색] : https://docs.github.com/ko/search-github/searching-on-github/searching-commits
- [검색 랭킹] : https://docs.github.com/ko/rest/search/search?apiVersion=2022-11-28#ranking-search-results
- [Gist 내용 업데이트] : https://docs.github.com/ko/rest/reference/gists#update-a-gist-comment

## Thanks for reading!
