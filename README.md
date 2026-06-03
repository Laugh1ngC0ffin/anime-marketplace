# 🎌 Anime Marketplace

Маркетплейс для покупки и продажи аниме товаров. Вдохновлено Авито, но специализировано на аниме.

## 📋 Функциональность

- ✅ Каталог аниме товаров
- ✅ Система поиска и фильтрации
- ✅ Профиль пользователя
- ✅ Создание объявлений
- ✅ Система рейтинга и отзывов
- ✅ Чат между продавцом и покупателем
- ✅ Безопасные платежи

## 🛠️ Технологический стек

| Компонент | Технология |
|-----------|-----------|
| Frontend | React + Vite + Tailwind CSS |
| Backend | Node.js + Express |
| Database | MongoDB |
| Auth | JWT |
| Hosting | Vercel (Frontend) + Render (Backend) |

## 🚀 Быстрый старт

### Требования
- Node.js 16+
- npm или yarn
- MongoDB (локально или MongoDB Atlas)

### Установка

#### 1. Клонируй репозиторий
```bash
git clone https://github.com/Laugh1ngC0ffin/anime-marketplace.git
cd anime-marketplace
```

#### 2. Установи зависимости

**Frontend:**
```bash
cd frontend
npm install
```

**Backend:**
```bash
cd ../backend
npm install
```

#### 3. Создай .env файлы

**backend/.env:**
```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/anime-marketplace
JWT_SECRET=your_secret_key_here
NODE_ENV=development
```

**frontend/.env:**
```
VITE_API_URL=http://localhost:5000
```

#### 4. Запусти приложение

**Backend (в папке backend):**
```bash
npm run dev
```

**Frontend (в папке frontend):**
```bash
npm run dev
```

Приложение будет доступно на `http://localhost:5173`

## 📁 Структура проекта

```
anime-marketplace/
├── frontend/
│   ├── src/
│   │   ├── components/      # React компоненты
│   │   ├── pages/          # Страницы
│   │   ├── styles/         # CSS файлы
│   │   ├── utils/          # Вспомогательные функции
│   │   └── App.jsx
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── models/             # MongoDB модели
│   ├── routes/             # API маршруты
│   ├── controllers/        # Логика приложения
│   ├── middleware/         # Middleware (auth и т.д.)
│   ├── config/             # Конфигурация
│   ├── server.js           # Точка входа
│   └── package.json
│
└── README.md
```

## 🔑 Основные возможности

### Для покупателей
- Просмотр каталога товаров
- Поиск по названию, категории, цене
- Просмотр отзывов продавца
- Безопасная коммуникация через чат
- История покупок

### Для продавцов
- Создание объявлений
- Управление товарами
- Просмотр статистики
- Рейтинг и отзывы

## 🧪 Тестирование API

Используй **Postman** или **curl** для тестирования API:

```bash
# Получить все товары
curl http://localhost:5000/api/products

# Получить товар по ID
curl http://localhost:5000/api/products/123

# Создать товар (требует авторизацию)
curl -X POST http://localhost:5000/api/products \
  -H "Content-Type: application/json" \
  -d '{"title": "Фигурка Асуны", "price": 2500, "category": "figurines"}'
```

## 📚 Документация

- [Frontend документация](./frontend/README.md) (будет добавлена)
- [Backend API документация](./backend/README.md) (будет добавлена)

## 🚨 Важные замечания

⚠️ **Это учебный проект!** Перед использованием в production:
- Добавь настоящую систему платежей
- Включи HTTPS
- Установи CORS правильно
- Добавь валидацию на всех уровнях
- Используй переменные окружения для всех секретов

## 📞 Поддержка

Если возникли проблемы, создай **Issue** в репозитории.

## 📄 Лицензия

MIT License

---

**Создано для обучения. Приятного кодирования!** 🚀
