---
📝 Level 2: GitHub 협업 실전훈련

GitHub에서 협업을 위한 브랜치 전략과 Pull Request(PR) 과정을 실무 관점에서 실습합니다.

상황:  
동료와 함께 프로젝트를 진행하며, 기능 개발을 위해 브랜치를 만들고 PR을 통해 코드를 병합합니다.

## 실습 목표

- 브랜치 생성 및 전환
- 기능 개발 후 커밋 및 푸시
- Pull Request(PR) 생성 및 병합
- 협업 시 코드 리뷰 흐름 이해

## 세부 지시사항

1. GitHub 저장소(github-branch-practice)를 클론하세요.
2. 터미널에서 저장소 폴더로 이동하세요.
3. feature/greet라는 새 브랜치를 생성하고 전환하세요.
4. greet.txt 파일을 생성하고 아래 내용을 추가하세요.
   ```
   Hello, GitHub Team!
   ```
5. greet.txt 파일을 스테이징하고, 커밋 메시지는 feat: greet 기능 추가로 커밋하세요.
6. feature/greet 브랜치를 원격 저장소에 푸시하세요.
7. GitHub 웹사이트에서 feature/greet 브랜치로 Pull Request(PR)을 생성하세요.
8. PR 생성 후, 본인이 직접 PR을 승인(merge)하세요.
9. master 브랜치로 전환 후, 최신 상태로 동기화하세요.
10. greet.txt 파일이 master 브랜치에도 반영되었는지 확인하세요.

## 과제 제출

아래 내용을 순서대로 저에게 보여주세요.

1. 터미널에 입력한 모든 Git 명령어
2. 6번에서 푸시한 브랜치명과 원격 저장소 주소
3. 8번에서 PR 생성 및 병합 완료 화면(캡처 또는 주요 정보)
4. 10번에서 master 브랜치에 greet.txt가 반영된 증거(파일 내용 등)

---

💡 실무 팁

- `git branch [브랜치명]`: 새 브랜치 생성
- `git checkout [브랜치명]`: 브랜치 전환
- `git checkout -b [브랜치명]`: 생성과 전환을 한 번에
- `git push -u origin [브랜치명]`: 새 브랜치 원격 푸시
- PR(Pull Request): 협업 시 코드 리뷰 및 병합 절차

궁금한 점이 있으면 언제든 질문해 주세요!

---

🏆 Level 2 실습 정답 예시

### 터미널에 입력한 Git 명령어

```bash
# 1. 저장소 클론 및 이동
git clone https://github.com/사용자명/github-branch-practice.git
cd github-branch-practice

# 2. 브랜치 생성 및 전환
git checkout -b feature/greet

# 3. 파일 생성 및 내용 추가
echo "Hello, GitHub Team!" > greet.txt

# 4. 파일 스테이징 및 커밋
git add greet.txt
git commit -m "feat: greet 기능 추가"

# 5. 브랜치 푸시
git push -u origin feature/greet
```

### 6번: 푸시한 브랜치명과 원격 저장소 주소 예시

- 브랜치명: feature/greet
- origin https://github.com/사용자명/github-branch-practice.git (fetch)
- origin https://github.com/사용자명/github-branch-practice.git (push)

### 8번: PR 생성 및 병합 완료 화면 예시

- PR 제목: feat: greet 기능 추가
- 상태: Merged
- 브랜치: feature/greet → master  
  (실제 화면 캡처를 첨부)

### 10번: master 브랜치에 greet.txt 반영 확인 예시

```bash
# master 브랜치로 전환 및 동기화
git checkout master
git pull origin master

# greet.txt 파일 내용 확인
cat greet.txt
# 출력: Hello, GitHub Team!
```

필요에 따라 파일명, 브랜치명, 메시지 등은 자유롭게 변경해도 됩니다.
