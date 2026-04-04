---
title: Git Workflow Tips
tags:
  - git
  - productivity
  - tips
date: 2026-03-25
---

Một số mẹo cải thiện Git workflow hàng ngày.

## Branch Naming Convention

- `feature/ten-tinh-nang` - Tính năng mới
- `bugfix/sua-loi` - Sửa lỗi
- `hotfix/urgent-fix` - Sửa lỗi khẩn cấp
- `refactor/toi-uu-code` - Refactor

## Commit Message Convention

Sử dụng [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: them tinh nang dang nhap
fix: sua loi validation form
docs: cap nhat README
refactor: toi uu ham xu ly
```

## Useful Commands

```bash
# Xem lịch sử commit dạng graph
git log --oneline --graph --all

# Stash thay đổi
git stash
git stash pop

# Undo commit cuối (giữ lại changes)
git reset --soft HEAD~1

# Squash commits
git rebase -i HEAD~3

# Xem diff giữa 2 branches
git diff main..feature-branch
```

## Git Hooks

Sử dụng Husky để setup pre-commit hooks:

```bash
npm install husky --save-dev
npx husky install
```

## Tips

1. **Commit thường xuyên** - Mỗi commit nên là một thay đổi nhỏ, độc lập
2. **Pull trước khi push** - Tránh conflict
3. **Dùng .gitignore** - Không commit file không cần thiết
4. **Review code** - Luôn review trước khi merge

---

> Xem thêm: [[notes]]
