# Driver POSNET для 1С:Enterprise - Landing Page

## 📋 Опис проекту

Сучасний лендінг для презентації та продажу зовнішньої компоненти "Driver POSNET" для інтеграції з фіскальними реєстраторами в системі 1С:Enterprise. Проект розроблений з використанням React, TypeScript, Tailwind CSS та Framer Motion.

## 🌍 Мультимовність

Сайт підтримує 3 мови:
- **Українська** (за замовчуванням)
- **Польська** 
- **Російська**

## ⚙️ Технічний стек

- **Frontend Framework:** React 18 + TypeScript
- **Build Tool:** Vite
- **Styling:** Tailwind CSS + shadcn/ui
- **Анімації:** Framer Motion
- **Іконки:** Phosphor Icons
- **Форми:** React Hook Form + Zod validation
- **Повідомлення:** Sonner toasts
- **SEO:** Structured Data (JSON-LD)

## 🚀 Встановлення та запуск

### Вимоги до системи
- Node.js 18+ 
- npm або yarn

### Крок 1: Клонування проекту
```bash
git clone [repository-url]
cd spark-template
```

### Крок 2: Встановлення залежностей
```bash
npm install
# або
yarn install
```

### Крок 3: Запуск в режимі розробки
```bash
npm run dev
# або
yarn dev
```

Проект буде доступний за адресою: `http://localhost:5173`

### Крок 4: Збірка для продакшн
```bash
npm run build
# або
yarn build
```

### Крок 5: Попередній перегляд збірки
```bash
npm run preview
# або
yarn preview
```

## 📂 Структура проекту

```
src/
├── components/           # React компоненти
│   ├── ui/              # shadcn/ui компоненти
│   ├── Header.tsx       # Хедер сайту
│   ├── Hero.tsx         # Головна секція
│   ├── Features.tsx     # Функціональні можливості
│   ├── Pricing.tsx      # Ціна та умови
│   ├── FAQ.tsx          # Часті питання
│   ├── Footer.tsx       # Футер сайту
│   ├── ContactModal.tsx # Модальне вікно зворотнього зв'язку
│   ├── ScrollToTop.tsx  # Кнопка прокрутки до верху
│   └── OwlMascot.tsx    # Корпоративний персонаж (сова)
├── hooks/               # Custom React hooks
│   ├── useTranslation.tsx # Система перекладів
│   ├── useSmoothScroll.ts # Плавна прокрутка
│   └── useInView.ts     # Відстеження появи елементів
├── lib/                 # Утиліти та конфігурації
│   ├── utils.ts         # Допоміжні функції
│   └── smoothScroll.ts  # Функції плавної прокрутки
├── assets/              # Статичні ресурси
│   ├── images/          # Зображення
│   ├── icons/           # Іконки
│   └── videos/          # Відео файли
├── App.tsx              # Головний компонент
├── main.tsx             # Точка входу
└── index.css            # Глобальні стилі
```

## 🎨 Дизайн система

### Кольорова палітра
- **Primary:** oklch(0.55 0.22 240) - Основний синій
- **Accent:** oklch(0.65 0.18 220) - Блакитний акцент
- **Background:** oklch(0.98 0.02 240) - Світлий фон
- **Text:** oklch(0.15 0.08 240) - Темний текст

### Шрифти
- **Основний:** Inter (Google Fonts)
- **Розміри:** 12px - 72px (адаптивні)

## 🔧 Основні функції

### ✅ Реалізовано
- [x] Адаптивний дизайн (мобільні, планшети, десктоп)
- [x] Мультимовність (UA/PL/RU)
- [x] SEO оптимізація
- [x] Плавна прокрутка та анімації
- [x] Форма зворотнього зв'язку
- [x] Віджет дзвінка (Zadarma)
- [x] Кнопка прокрутки до верху
- [x] Cookie consent
- [x] Політика приватності
- [x] Structured Data для пошукових систем

### 🎭 Анімації та UX
- Smooth scroll з уніфікованими налаштуваннями
- Hover ефекти для всіх інтерактивних елементів
- Анімований корпоративний персонаж (сова)
- Модальні вікна з адаптивною версткою
- Lazy loading для оптимізації продуктивності

## 🌐 SEO Оптимізація

### Структуровані дані
- Organization schema
- Product schema  
- LocalBusiness schema
- FAQ schema
- WebSite schema

### Meta теги
- Open Graph для соцмереж
- Twitter Card
- Canonical URLs
- Hreflang для мультимовності
- Optimized meta descriptions

## 📱 Адаптивність

Повністю адаптивний дизайн з брейкпоінтами:
- **Mobile:** < 768px
- **Tablet:** 768px - 1024px  
- **Desktop:** > 1024px

## 🔗 Інтеграції

### Zadarma Віджет
- Віджет дзвінка для швидкого зв'язку
- Мобільна адаптація
- Кастомна стилізація

### Google Analytics
- GA4 інтеграція
- Enhanced ecommerce tracking
- Custom events

## 🚦 Оптимізація продуктивності

- **Code Splitting:** Lazy loading компонентів
- **Image Optimization:** WebP формат + lazy loading
- **CSS Optimization:** Critical CSS inline
- **Bundle Optimization:** Tree shaking
- **Preloading:** Critical resources

## 🛠 Команди для розробки

```bash
# Запуск dev сервера
npm run dev

# Збірка проекту
npm run build

# Попередній перегляд збірки
npm run preview

# Перевірка типів TypeScript
npm run type-check

# Лінтинг коду
npm run lint

# Форматування коду
npm run format
```

## 📋 Todo / Розширення функціоналу

- [ ] Інтеграція з CRM системою
- [ ] A/B тестування
- [ ] Чат-бот підтримка
- [ ] Відгуки клієнтів
- [ ] Блог секція
- [ ] Демо-версія продукту

## 📞 Контактна інформація

**ModulSoft**
- 📍 43025, м. Луцьк, вул. Святовасилівська 4/3
- ☎️ +38 (093) 177-65-04  
- 📧 info@modulsoft.eu
- 🌐 https://posnet.modulsoft.eu

## 📝 Ліцензія

© 2025 ModulSoft. Всі права захищені.

---

**Розробник:** ModulSoft Development Team  
**Версія:** 1.0.0  
**Останнє оновлення:** Січень 2025