---
title: Стандарты и кодирования React Native на TypeScript
categories:
  - chudnyi
description: Стандарты и практики кодирования проекта мобильного приложения React Native на TypeScript
type: Document
author: chudnyi
---

## render

#### R101

- ❌ Использовать `EStyleSheet.value('$color.text.base')` в `render`
- ✅ Использовать `SS.$trendPositive` в `render`
```ts
const SS = EStyleSheet.create({
  $trendPositive: '$color.good.base',
});
```

## import/export

#### R201

- ✅ Файл `index.ts` должен экспортировать из папки только простые независимые типы и интерфейсы
- ❌ Файл `index.ts` не должен экспортировать из папки классы-реализации сервисов и сторов

## types

#### R301

- ✅ Используй `undefined` вместо `null`
- ❌ Не используй `null`, кроме случаев, когда без него не обойтись

## Комментарии

#### R401

- Если строка вывода лога должна остаться к коде, необходио пометитьеё значками: 🐞 ✅. Например: `console.log('BIO ERROR: ', error); // 🐞 ✅`
