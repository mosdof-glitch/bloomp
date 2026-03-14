# 🚗 BLOOMP - Complete Flutter Project

> AI-powered маркетплейс автозапчастей для Казахстана

---

## 📦 СТРУКТУРА ПРОЕКТА

```
bloomp/
├── pubspec.yaml                 # Зависимости
├── .env.example                 # Шаблон для API ключей
├── .gitignore
├── README.md
│
├── android/                     # Android конфигурация
├── ios/                         # iOS конфигурация
├── web/                         # Web конфигурация
│
└── lib/                         # 🎯 ВЕСЬ КОД ЗДЕСЬ
    ├── main.dart                # Точка входа
    │
    ├── core/                    # Ядро
    │   ├── theme/
    │   │   └── app_colors.dart
    │   ├── providers/
    │   │   ├── auth_provider.dart
    │   │   ├── cart_provider.dart
    │   │   ├── favorites_provider.dart
    │   │   └── garage_provider.dart
    │   ├── services/
    │   │   ├── supabase_service.dart
    │   │   ├── garage_service.dart
    │   │   ├── gemini_service.dart
    │   │   └── excel_service.dart
    │   └── data/
    │       ├── car_data.dart
    │       └── mock_products.dart
    │
    ├── shared/                  # Общие компоненты
    │   ├── models/
    │   │   ├── user.dart
    │   │   ├── product.dart
    │   │   ├── cart_item.dart
    │   │   └── garage_vehicle.dart
    │   └── widgets/
    │       ├── brand_model_picker.dart
    │       ├── year_picker.dart
    │       └── ai_recommendations.dart
    │
    └── features/                # Экраны приложения
        ├── home/
        │   └── screens/
        │       ├── splash_screen.dart
        │       └── home_screen.dart
        ├── catalog/
        │   └── screens/
        │       ├── catalog_screen.dart
        │       └── product_detail_screen.dart
        ├── cart/
        │   └── screens/
        │       ├── cart_screen.dart
        │       ├── checkout_screen.dart
        │       └── order_success_screen.dart
        ├── profile/
        │   └── screens/
        │       ├── profile_screen.dart
        │       └── settings_screen.dart
        ├── favorites/
        │   └── screens/
        │       └── favorites_screen.dart
        ├── auth/
        │   └── screens/
        │       ├── login_screen.dart
        │       ├── register_screen.dart
        │       └── sms_verification_screen.dart
        ├── garage/
        │   └── screens/
        │       ├── garage_screen.dart
        │       └── add_vehicle_screen.dart
        ├── search/
        │   └── screens/
        │       ├── image_search_screen.dart
        │       └── voice_search_screen.dart
        ├── chat/
        │   └── screens/
        │       └── chatbot_screen.dart
        └── admin/
            └── screens/
                └── export_catalog_screen.dart
```

---

## 🚀 УСТАНОВКА

### 1. Требования

```bash
Flutter SDK: >= 3.0.0
Dart SDK: >= 3.0.0
```

### 2. Клонируй и установи зависимости

```bash
# Установи зависимости
flutter pub get

# Проверь
flutter doctor
```

### 3. Настрой .env

```bash
# Скопируй шаблон
cp .env.example .env

# Добавь свои ключи
GEMINI_API_KEY=your_gemini_key_here
SUPABASE_URL=your_supabase_url_here
SUPABASE_ANON_KEY=your_supabase_anon_key_here
```

### 4. Запусти

```bash
# Android
flutter run

# iOS
flutter run -d ios

# Web
flutter run -d chrome
```

---

## 📝 КЛЮЧЕВЫЕ ФАЙЛЫ

См. папку `lib/` для всех исходников.

**Файлы готовы к копированию!**

---

## 🔑 MOCK DATA

### Авторизация:
- Любой телефон + пароль >= 6 символов
- SMS код: **123456**

### Тестовые аккаунты:
- Buyer: +7 777 111 22 33 / demo123
- Seller: +7 777 444 55 66 / seller123

---

## 🎯 ОСНОВНЫЕ ФУНКЦИИ

✅ WhatsApp/SMS авторизация  
✅ AI поиск по фото (Gemini Vision)  
✅ Голосовой поиск  
✅ AI-чат помощник  
✅ Мой гараж (CRUD авто)  
✅ Корзина с Hive persistence  
✅ Избранное  
✅ Каталог с фильтрами  
✅ Seller cabinet  
✅ Excel export  

---

## 📚 ЗАВИСИМОСТИ

См. `pubspec.yaml` для полного списка.

**Основные:**
- provider (state management)
- hive (local storage)
- google_generative_ai (Gemini AI)
- supabase_flutter (backend)
- image_picker (camera)
- speech_to_text (voice)
- excel (export)

---

## 🎨 ЦВЕТА БРЕНДА

- Primary: #F91155 (розовый)
- Secondary: #2E6FF2 (синий)
- WhatsApp: #25D366 (зеленый)

---

## 📞 ПОДДЕРЖКА

Email: azamat@bloomp.kz  
Telegram: @azamat_bloomp

---

**BLOOMP v1.0 | March 2026**
