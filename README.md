# 도서 관리 앱

*(이 README는 GitHub Copilot CLI를 사용하여 개선할 수 있도록 의도적으로 다듬어지지 않았습니다.)*

소유하고 있거나 읽고 싶은 책을 관리하는 Python 앱입니다.

책을 추가, 삭제, 목록 보기할 수 있으며, 읽음 표시도 가능합니다.

---

## 현재 기능

* JSON 파일(데이터베이스)에서 책 정보를 읽어옵니다.
* 일부 입력 검사가 미흡합니다.
* 테스트가 일부 존재하지만 충분하지 않을 수 있습니다.

---

## 파일

* `book_app.py` - 메인 CLI 진입점
* `books.py` - 데이터 로직을 포함하는 BookCollection 클래스
* `utils.py` - UI 및 입력 관련 헬퍼 함수
* `data.json` - 샘플 책 데이터
* `tests/test_books.py` - pytest 테스트 시작 파일

---

## 앱 실행

```bash
python book_app.py list
python book_app.py add
python book_app.py find
python book_app.py remove
python book_app.py help
```

## 테스트 실행

```bash
python -m pytest tests/
```

---

## 참고 사항

* 해당 없음 실제 사용 가능한 수준 (당연히)
* 일부 코드는 개선될 여지가 있습니다.
* 나중에 명령어를 더 추가할 수 있습니다.  

```bash
python book_app.py add

Title: Harry Potter and the Philosopher's Stone  
Author: J.K. Rowling  
Year: 1997  
```

## Running Tests
Ask Copilot CLI a plain-English question about your toolchain. It can generate the right shell command for you.
```
copilot

> How do I run the tests? Show me the pytest command.

# Copilot CLI responds:
# python -m pytest tests/
# Or for verbose output: python -m pytest tests/ -v
# To see print statements: python -m pytest tests/ -s
```