qa-photo-uploader/

├── qa_upload_form_final.html      ← 업로드용 HTML 폼

├── qa_data/                       ← JSON + 사진 저장 폴더

├── reports/                       ← Excel 리포트 저장 폴더

├── credentials.json               ← Google API 인증파일 (업로드 시 제외)

├── upload_to_gdrive.py

├── generate_excel_report.py

├── run_qa_tool.py

├── README.md                      ← 사용법 설명서



# 📷 QA Photo Uploader

## 기능
- GOOD / BAD 사진 각각 1~5장 업로드
- COMPANY, FACTORY, ITEM, STYLECODE, MO 등 필드 입력
- 선택된 DEFECT DESC 포함한 JSON 저장
- Google Drive 자동 업로드
- Excel 자동 리포트 생성

## 사용 방법

1. `qa_upload_form_final.html` 실행 → JSON + 사진 저장
2. `run_qa_tool.py` 실행 → 자동 업로드 + 리포트 생성

## 필요 패키지

```bash
pip install pydrive2 pandas openpyxl tk


---

## 📌 GitHub에 업로드 방법 (직접 하시는 경우)

1. GitHub에서 새 저장소 생성: `qa-photo-uploader`
2. 로컬에서 폴더 구성 후 아래 실행

```bash
git init
git remote add origin https://github.com/yourname/qa-photo-uploader.git
git add .
git commit -m "Initial commit: QA Uploader"
git push -u origin main
