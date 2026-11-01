# 시험 키트

에이전트가 읽고 실행하는 셋업 절차다. 이 파일(`KIT.md`)은 작업 공간에 복사하지 않는다.

## 셋업 절차

1. 양식을 가져온다. `-n`은 이미 있는 파일을 덮어쓰지 않는다.
   ```bash
   git clone --depth 1 https://github.com/sfbluejihwan/exam-preparation /tmp/kit
   cp -n /tmp/kit/AGENTS.md /tmp/kit/SPEC.md /tmp/kit/VERIFY.md .
   ```
2. 작업 공간에 AGENTS.md가 이미 있었으면 덮어쓰지 않고 `/tmp/kit/AGENTS.md` 내용을 그 뒤에 덧붙인다.
3. `rm -rf /tmp/kit`
