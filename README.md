# Next Pizza

Веб-приложение для заказа пиццы, построенное с использованием современных технологий и инструментов.

## Описание проекта

**Next Pizza** — это полнофункциональное приложение для онлайн-заказа пиццы. Проект демонстрирует лучшие практики разработки на Next.js 16 с использованием TypeScript, Tailwind CSS и компонентов Shadcn UI.

### Основные возможности

- **Каталог продуктов** — просмотр доступных пицц и других товаров
- **Корзина покупок** — управление заказом перед оплатой
- **Современный UI** — отзывчивый дизайн на основе Tailwind CSS и Shadcn UI
- **Оптимизированная производительность** — использование Next.js App Router
- 🔧 **TypeScript** — полная типизация кода для надежности

## Технологический стек

- **Frontend Framework**: [Next.js 16.2.3](https://nextjs.org/) — React-фреймворк с интегрированной оптимизацией
- **UI/React**: [React 19.2.4](https://react.dev/) — библиотека для создания пользовательских интерфейсов
- **Язык программирования**: [TypeScript 5](https://www.typescriptlang.org/) — типизированный JavaScript
- **Стилизация**: 
  - [Tailwind CSS 4.2.2](https://tailwindcss.com/) — утилит-фреймворк для CSS
  - [tailwindcss-animate](https://github.com/jamiebuilds/tailwindcss-animate) — анимации для Tailwind
- **Компоненты UI**: 
  - [Shadcn UI](https://ui.shadcn.com/) — переиспользуемые компоненты React
  - [Radix UI](https://www.radix-ui.com/) — примитивы для создания доступных компонентов
- **Утилиты**:
  - [Lucide React](https://lucide.dev/) — библиотека иконок
  - [clsx](https://github.com/lukeed/clsx) — управление классами CSS
  - [tailwind-merge](https://github.com/dcastil/tailwind-merge) — слияние Tailwind классов
  - [Vaul](https://vaul.emilkowalski.com/) — компонент Drawer

## Структура проекта

```
next-pizza/
├── app/                    # App Router приложения
│   ├── layout.tsx          # Корневой layout
│   ├── page.tsx            # Главная страница
│   ├── globals.css         # Глобальные стили
│   └── product/
│       └── [id]/
│           └── page.tsx    # Страница продукта
├── components/             # React компоненты
│   ├── shared/             # Переиспользуемые компоненты
│   │   ├── header.tsx      # Заголовок приложения
│   │   ├── container.tsx   # Контейнер-обертка
│   │   └── index.ts        # Экспорты
│   └── ui/                 # UI компоненты (Shadcn)
│       ├── button.tsx
│       ├── dialog.tsx
│       ├── drawer.tsx
│       ├── input.tsx
│       ├── select.tsx
│       └── ...
├── lib/                    # Утилиты и вспомогательные функции
│   └── utils.ts            # Утилиты (cn() для классов)
├── public/                 # Статические файлы
│   └── assets/
│       └── images/         # Изображения
├── next.config.ts          # Конфигурация Next.js
├── tailwind.config.ts      # Конфигурация Tailwind CSS
├── tsconfig.json           # Конфигурация TypeScript
└── package.json            # Зависимости проекта
```

## Установка и запуск

### Требования

- Node.js 18+ или выше
- npm, yarn, pnpm или bun

### Шаги установки

1. **Клонируйте репозиторий**:
   ```bash
   git clone <repository-url>
   cd next-pizza
   ```

2. **Установите зависимости**:
   ```bash
   npm install
   ```

3. **Запустите сервер разработки**:
   ```bash
   npm run dev
   ```

   Сервер будет доступен по адресу [http://localhost:3000](http://localhost:3000)

4. **Откройте в браузере**:
   Перейдите на [http://localhost:3000](http://localhost:3000) чтобы увидеть приложение

## Доступные команды

```bash
# Запуск сервера разработки
npm run dev

# Сборка для продакшена
npm run build

# Запуск продакшена
npm start

# Проверка кода ESLint
npm run lint
```

## Разработка

### Добавление новых компонентов

Компоненты Shadcn UI можно добавить с помощью CLI:
```bash
npx shadcn-ui@latest add [component-name]
```

### Структурирование стилей

Используется Tailwind CSS с поддержкой анимаций. Глобальные стили находятся в `app/globals.css`.

### TypeScript типы

Проект полностью типизирован с использованием TypeScript 5. Типы для React компонентов добавлены через `@types/react`.

## Развертывание

### На Vercel (рекомендуется)

Самый простой способ развернуть приложение:

1. Откройте [Vercel Platform](https://vercel.com/)
2. Подключите ваш GitHub репозиторий
3. Vercel автоматически обнаружит Next.js и сконфигурирует развертывание

### На других платформах

Используйте команду для сборки:
```bash
npm run build
npm start
```

## Ресурсы

- [Документация Next.js](https://nextjs.org/docs)
- [Learn Next.js](https://nextjs.org/learn)
- [Shadcn UI Documentation](https://ui.shadcn.com/)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [React Documentation](https://react.dev/)

## Лицензия

Этот проект лицензирован под MIT лицензией.

---

**Автор**: Next Pizza Team  
**Версия**: 0.1.0  
**Статус**: Завершен
