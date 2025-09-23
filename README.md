# Driver POSNET для 1С:Enterprise - Landing Page

Професійний лендінг для продажу компоненти інтеграції фіскальних реєстраторів POSNET з системою 1С:Enterprise.

## 🚀 Особливості

- **Багатомовність**: Підтримка української, польської та російської мов
- **Адаптивний дизайн**: Оптимізований для всіх пристроїв
- **SEO оптимізація**: Повна структурована розмітка та метадані
- **Анімації**: Плавні переходи та інтерактивні елементи
- **Швидкодія**: Оптимізовано для максимальної продуктивності
- **Віджет зворотного зв'язку**: Інтеграція з Zadarma

## 🛠 Технології

- **React 18** + **TypeScript**
- **Vite** - швидка збірка та dev server
- **Tailwind CSS** - утилітарні CSS класи
- **Framer Motion** - анімації та переходи
- **Shadcn/ui** - компоненти UI
- **Sonner** - сповіщення (toast)
- **Phosphor Icons** - набір іконок

## 📋 Системні вимоги

Перед запуском переконайтеся, що у вас встановлено:

- **Node.js** версія 18.0.0 або новіша
- **npm** версія 8.0.0 або новіша (або **yarn**/**pnpm**)
- **Git** для клонування репозиторію

### Перевірка версій:
```bash
node --version
npm --version
git --version
```

## 🔧 Локальний запуск

### 1. Клонування репозиторію

```bash
# Клонування проекту
git clone <URL_РЕПОЗИТОРІЮ>
cd spark-template
```

### 2. Встановлення залежностей

```bash
# Встановлення всіх npm пакетів
npm install

# Або якщо використовуєте yarn
yarn install

# Або якщо використовуєте pnpm
pnpm install
```

### 3. Запуск в режимі розробки

```bash
# Запуск dev сервера
npm run dev

# Або з yarn
yarn dev

# Або з pnpm
pnpm dev
```

Після запуску проект буде доступний за адресою: **http://localhost:5173**

### 4. Збірка для продакшну

```bash
# Збірка оптимізованої версії
npm run build

# Перегляд зібраної версії локально
npm run preview
```

## 📁 Структура проекту

```
spark-template/
├── public/                 # Статичні файли
│   ├── favicon.svg
│   └── ...
├── src/                    # Вихідний код
│   ├── components/         # React компоненти
│   │   ├── ui/            # Shadcn UI компоненти
│   │   ├── Header.tsx
│   │   ├── Hero.tsx
│   │   ├── Features.tsx
│   │   └── ...
│   ├── hooks/             # React hooks
│   │   ├── useTranslation.tsx
│   │   ├── useSmoothScroll.ts
│   │   └── ...
│   ├── lib/               # Утиліти
│   │   └── utils.ts
│   ├── utils/             # Додаткові утиліти
│   │   └── optimization.ts
│   ├── App.tsx            # Головний компонент
│   ├── index.css          # Стилі
│   └── main.tsx           # Точка входу
├── index.html             # HTML шаблон
├── package.json           # Конфігурація npm
├── tailwind.config.js     # Конфігурація Tailwind
├── tsconfig.json          # Конфігурація TypeScript
├── vite.config.ts         # Конфігурація Vite
└── README.md              # Цей файл
```

## 🎨 Кольорова схема

Проект використовує синьо-блакитну палітру:

- **Primary**: `oklch(0.55 0.22 240)` - основний синій
- **Accent**: `oklch(0.65 0.18 220)` - блакитний акцент
- **Background**: `oklch(0.98 0.02 240)` - світлий фон
- **Foreground**: `oklch(0.15 0.08 240)` - темний текст

## 🌍 Багатомовність

Проект підтримує 3 мови:
- **Українська** (за замовчуванням)
- **Польська**
- **Російська**

Переклади зберігаються в `src/hooks/useTranslation.tsx`. Для додавання нових перекладів:

1. Відкрийте файл `src/hooks/useTranslation.tsx`
2. Додайте нові ключі в об'єкти `translations`
3. Використовуйте в компонентах: `const { t } = useTranslation()`

## 🔧 Налаштування

### Заміна контактної інформації

Відредагуйте файли:
- `src/components/ContactPage.tsx` - сторінка контактів
- `src/components/Footer.tsx` - футер
- `index.html` - мета-теги з контактами

### Налаштування Zadarma віджета

В файлі `index.html` замініть:
```javascript
var ZCallbackWidgetLinkId = 'YOUR_ZADARMA_ID';
```

### Налаштування аналітики

В файлі `index.html` замініть:
- `GA_MEASUREMENT_ID` - на ваш Google Analytics ID
- `CLARITY_PROJECT_ID` - на ваш Microsoft Clarity ID
- `HOTJAR_ID` - на ваш Hotjar ID

## 🚀 Деплой

### Vercel (рекомендовано)
```bash
npm i -g vercel
vercel --prod
```

### Netlify
```bash
npm run build
# Завантажте папку dist/ в Netlify
```

### GitHub Pages
```bash
npm run build
# Налаштуйте GitHub Actions для деплою з папки dist/
```

## 🐛 Відладка

### Поширені проблеми:

**Помилка при запуску dev сервера:**
```bash
# Очистіть кеш і переустановіть залежності
rm -rf node_modules package-lock.json
npm install
npm run dev
```

**Проблеми з TypeScript:**
```bash
# Перевірка типів
npm run build
```

**Проблеми зі стилями:**
```bash
# Перезапустіть Tailwind процес
npm run dev
```

## 📊 Продуктивність

Проект оптимізовано для швидкого завантаження:

- **Lazy loading** компонентів
- **Image optimization** 
- **Code splitting**
- **Preload критичних ресурсів**
- **SEO оптимізація**

### Моніторинг продуктивності:
```bash
# Аналіз bundle
npm run build -- --analyze

# Lighthouse аудит в браузері:
# DevTools > Lighthouse > Generate report
```

## 🤝 Внесок у розробку

1. Зробіть fork репозиторію
2. Створіть feature branch: `git checkout -b feature/amazing-feature`
3. Зробіть commit: `git commit -m 'Add amazing feature'`
4. Push у branch: `git push origin feature/amazing-feature`
5. Відкрийте Pull Request

## 📝 Ліцензія

© 2025 ModulSoft. Всі права захищені.

---

## 🔗 Корисні посилання

- [Vite Documentation](https://vitejs.dev/)
- [React Documentation](https://react.dev/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Framer Motion](https://www.framer.com/motion/)
- [Shadcn/ui](https://ui.shadcn.com/)

## 📞 Підтримка

Якщо у вас виникли питання або проблеми:

- **Email**: info@modulsoft.eu
- **Телефон**: +38 (093) 177-65-04
- **Сайт**: https://modulsoft.eu

---

**Версія проекту**: 2.0  
**Остання оновлення**: Січень 2025