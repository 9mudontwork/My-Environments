# zip ไฟล์ ที่แก้ไขทั้งหมด between commit

```text
git archive --output=archived_changes.zip new-srb-dev $(git diff --diff-filter=ACMRTUXB --name-only 57bd8c7 ef6e175)
```

