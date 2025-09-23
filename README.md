# Driver POSNET для 1С:Enterprise - Landing Page

Професійний багатомовний лендінг для продажу зовнішньої компоненти інтеграції POSNET реєстраторів з системою 1С:Enterprise.

## 🚀 Особливості проекту

- **Багатомовність**: Підтримка української, польської та російської мов
- **Адаптивний дизайн**: Оптимізовано для всіх пристроїв (мобільні, планшети, десктопи)
- **SEO-оптимізація**: Повна оптимізація для пошукових систем з підтримкою множини мов
- **Продуктивність**: Оптимізована швидкість завантаження та Web Vitals
- **Інтерактивність**: Анімації, модальні вікна, плавний скрол
- **Інтеграції**: Заdarma віджет зворотного зв'язку, аналітика

## 🛠 Технологічний стек

- **Framework**: Vite + React 18 + TypeScript
- **Стилізація**: Tailwind CSS + Shadcn/ui компоненти
- **Анімації**: Framer Motion
- **Іконки**: Phosphor Icons
- **Сповіщення**: Sonner (toast notifications)
- **SEO**: Структуровані дані (JSON-LD), Open Graph, Twitter Cards

## 📋 Передумови

Перед запуском проекту переконайтеся, що у вас встановлено:

- **Node.js** версії 18.0.0 або новіша
- **npm** версії 9.0.0 або новіша (або **yarn**/**pnpm**)
- **Git** для клонування репозиторію

## 🚀 Встановлення та запуск

### 1. Клонування репозиторію

```bash
git clone https://github.com/your-username/posnet-driver-landing.git
cd posnet-driver-landing
```

### 2. Встановлення залежностей

```bash
npm install
# або
yarn install
# або
pnpm install
```

### 3. Запуск у режимі розробки

```bash
npm run dev
# або
yarn dev
# або
pnpm dev
```

Проект буде доступний за адресою: `http://localhost:5173`

### 4. Збірка для продакшну

```bash
npm run build
# або
yarn build
# або
pnpm build
```

### 5. Превʼю збірки

```bash
npm run preview
# або
yarn preview
# або
pnpm preview
```

## 📁 Структура проекту

```
src/
├── components/           # React компоненти
│   ├── ui/              # Shadcn/ui базові компоненти
│   ├── Header.tsx       # Шапка сайту
│   ├── Hero.tsx         # Головна секція
│   ├── Features.tsx     # Функціональність
│   ├── Pricing.tsx      # Ціноутворення
│   ├── FAQ.tsx          # Часті питання
│   ├── Footer.tsx       # Підвал
│   └── ...              # Інші компоненти
├── hooks/               # React хуки
│   ├── useTranslation.tsx # Багатомовність
│   ├── useSmoothScroll.tsx # Плавний скрол
│   └── ...              # Інші хуки
├── utils/               # Утиліти
│   └── optimization.ts  # SEO та продуктивність
├── App.tsx              # Головний компонент додатку
├── index.css           # Глобальні стилі
└── main.tsx            # Точка входу
```

## 🌍 Багатомовність

Проект підтримує три мови:
- **Українська** (за замовчуванням) - `uk`
- **Польська** - `pl` 
- **Російська** - `ru`

### Додавання нових перекладів

1. Відредагуйте файл `src/hooks/useTranslation.tsx`
2. Додайте переклади для всіх ключів у відповідних мовних об'єктах
3. Переконайтеся, що всі компоненти використовують функцію `t()` для перекладів

## 🎨 Налаштування дизайну

### Кольорова схема

Проект використовує сині та блакитні відтінки. Змінити кольори можна в файлі `src/index.css`:

```css
:root {
  --background: oklch(0.98 0.02 240);
  --foreground: oklch(0.15 0.08 240);
  --primary: oklch(0.55 0.22 240);
  --accent: oklch(0.65 0.18 220);
  /* ... інші кольори */
}
```

### Шрифти

Проект використовує шрифт **Inter** від Google Fonts. Змінити шрифт можна в файлах:
- `index.html` - посилання на Google Fonts
- `src/index.css` - CSS правила для шрифту

## 📱 Адаптивність

Проект повністю адаптивний з брейкпоінтами:
- **Mobile**: до 768px
- **Tablet**: 768px - 1024px  
- **Desktop**: від 1024px

## ⚡ Оптимізація продуктивності

### Рекомендації для кращої продуктивності:

1. **Зображення**:
   - Використовуйте формат WebP для зображень
   - Оптимізуйте розмір зображень для різних пристроїв
   - Використовуйте lazy loading для зображень нижче складки

2. **Шрифти**:
   - Шрифти завантажуються асинхронно з `font-display: swap`
   - Критичні шрифти попередньо завантажуються

3. **JavaScript**:
   - Компоненти розділені на чанки для ленивого завантаження
   - Використовується React.memo для оптимізації ререндерів

## 🔧 Конфігурація

### Важливі налаштування:

1. **Zadarma віджет**: Налаштуйте ідентифікатор у файлі `index.html`
2. **Google Analytics**: Замініть `GA_MEASUREMENT_ID` на справжній ID
3. **SEO**: Оновіть метатеги в `index.html` під ваш домен

### Змінні середовища

Створіть файл `.env.local` для локальних налаштувань:

```env
VITE_API_BASE_URL=https://api.modulsoft.eu
VITE_GA_ID=GA_MEASUREMENT_ID
VITE_ZADARMA_WIDGET_ID=your_widget_id
```

## 🚀 Деплой

### Статичний хостинг (Netlify, Vercel)

1. Підʼєднайте репозиторій до платформи
2. Налаштуйте команди збірки:
   - Build command: `npm run build`
   - Publish directory: `dist`
3. Додайте змінні середовища у налаштуваннях проекту

### Apache/Nginx

1. Зберіть проект: `npm run build`
2. Скопіюйте вміст папки `dist/` на сервер
3. Налаштуйте веб-сервер для SPA (Single Page Application):

**Apache (.htaccess)**:
```apache
RewriteEngine On
RewriteBase /
RewriteRule ^index\.html$ - [L]
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule . /index.html [L]
```

**Nginx**:
```nginx
location / {
    try_files $uri $uri/ /index.html;
}
```

## 🔍 SEO оптимізація

### Автоматичні функції:
- Структуровані дані (JSON-LD)
- Open Graph мета-теги
- Twitter Card мета-теги
- Sitemap.xml генерація
- Багатомовні hreflang теги

### Ручне налаштування:
1. Оновіть `title` і `meta description` в `index.html`
2. Додайте зображення для Open Graph у папку `public/`
3. Налаштуйте Google Search Console і Analytics

## 📊 Моніторинг та аналітика

### Підключені сервіси:
- **Google Analytics 4**: Відстеження відвідувачів і конверсій
- **Microsoft Clarity**: Аналіз поведінки користувачів
- **Hotjar**: Теплові карти та записи сесій (опціонально)

### Web Vitals моніторинг:
Проект автоматично відстежує ключові метрики продуктивності:
- LCP (Largest Contentful Paint)
- FID (First Input Delay)  
- CLS (Cumulative Layout Shift)
- FCP (First Contentful Paint)
- TTFB (Time To First Byte)

## 🛠 Розробка

### Корисні команди:

```bash
# Запуск у режимі розробки
npm run dev

# Збірка для продакшну
npm run build

# Превʼю збірки
npm run preview

# Лінтинг коду
npm run lint

# Форматування коду
npm run format

# Перевірка типів TypeScript
npm run type-check
```

### Налагодження:

1. Використовуйте React DevTools для відлагодження компонентів
2. Web Vitals метрики виводяться в консоль браузера (у режимі розробки)
3. SEO health check доступний через `performSEOHealthCheck()` у консолі

## 📞 Підтримка

Для питань щодо розробки або деплою:

- **Email**: info@modulsoft.eu
- **Телефон**: +38 (093) 177-65-04
- **Сайт**: https://modulsoft.eu

## 📄 Ліцензія

© 2025 ModulSoft. Всі права захищені.

---

**Примітка**: Переконайтеся, що замінили всі заповнювачі (як-от `GA_MEASUREMENT_ID`, `HOTJAR_ID`, тощо) на реальні значення перед деплоєм у продакшн.