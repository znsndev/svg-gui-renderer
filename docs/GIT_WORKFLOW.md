# Git Workflow Guide

## 🌿 Branches (Ветки)

### Main branches (Основные ветки)

- `main` - production ready code (стабильная версия для релизов)
- `dev` - integration branch (основная ветка разработки)

### Temporary branches

- `feat/*` - new functionality (новая функциональность) (e.g. `feat/svg/button`)
- `fix/*` - bug fix (исправление багов) (e.g. `fix/button-click`)
- `hotfix/*` - urgent production fixes (срочные исправления) (e.g. `hotfix/critical-error`)
- `docs/*` - documentation updates (обновление документации) (e.g. `docs/api-reference`)

## 🚀 Development Process (Процесс разработки)

### Starting new feature (Начало новой функции)

```bash
# Update develop (Обновляем develop)
git checkout develop
git pull origin develop

# Create feature branch (Создаем feature ветку)
git checkout -b feature/component-name

# Work and commit regularly (Работаем и коммитим)
git add .
git commit -m "feat(buttons): add SVG button support"
```

### Completing feature [Завершение функции]:

```bash
# Push branch (Пушим ветку])
git push -u origin feature/component-name

# Create Pull Request feature → develop (Создаем PR)
# Complete code review (Проходим ревью)
# Merge and DELETE branch (Мержим и УДАЛЯЕМ ветку)
```

## Commit convention (Стандарт коммитов)

### Format (Формат)

    type(scope): brief description (тип(область): описание)

### Commit Types (Типы коммитов)
    
- `feat` - new feature (новая функциональность)
- `fix` - bug fix (исправление бага)
- `docs` - documentation changes (изменения документации)
- `style` - code style changes (изменения стиля кода)
- `refactor` - code refactoring (рефакторинг кода)
- `test` - adding tests (добавление тестов)
- `chore` - build process changes (изменения процесса сборки)

### Examples (Примеры)

```bash
git commit -m "feat(buttons): add hover state support"
git commit -m "fix(rendering) resolve SVG scaling"
git commit -m "docs(readme): update installation instructions"
```

--------------------------------

**Last Update:** _09.22.2025_

**Maintainers:** [MYP3UJIKA111](https://github.com/MYP3UJIKA111), [znsndev](https://github.com/znsndev)

> 💡 Note: This document should be updated as our workflow evolves
> 
>💡 Примечание: Этот документ должен обновляться по мере развития нашего workflow