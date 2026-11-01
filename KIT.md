# 시험 키트

작업 공간 루트에 둘 `AGENTS.md`·`SPEC.md`·`VERIFY.md` 양식이다. 이 파일(`KIT.md`)은 작업 공간에 복사하지 않는다.

## 시험장에서

1. 이 저장소를 clone해 써도 되는지 Cofa Helper에게 먼저 묻는다. 안 되면 카드를 보고 양식을 손으로 적는다.
2. 양식을 가져온다. `-n`은 이미 있는 파일을 덮어쓰지 않는다.
   ```bash
   git clone --depth 1 <이 저장소 URL> /tmp/kit
   cp -n /tmp/kit/AGENTS.md /tmp/kit/SPEC.md /tmp/kit/VERIFY.md .
   rm -rf /tmp/kit
   ```
3. 과제가 `AGENTS.md`를 제공했으면 덮어쓰지 않고 `/tmp/kit/AGENTS.md` 내용을 그 뒤에 덧붙인다(2의 `rm` 전에).
4. 공개 스킬을 가져온 뒤 Codex를 다시 시작하고 `$grill-with-docs`로 부른다.
   ```bash
   git clone --depth 1 https://github.com/mattpocock/skills /tmp/mps
   mkdir -p .agents/skills
   cp -r /tmp/mps/skills/engineering/grill-with-docs /tmp/mps/skills/productivity/grilling /tmp/mps/skills/engineering/domain-modeling .agents/skills/
   rm -rf /tmp/mps
   ```
5. 과제가 제출 문서의 이름·양식을 정하면 그 파일이 `SPEC.md`·`VERIFY.md`를 대신하고, `AGENTS.md`의 파일 위치 줄을 고친다.
