# ArtGallary 🖼️

Desktop-приложение для управления данными галереи искусств.

> ⚠️ Проект в стадии разработки (WIP) — реализован базовый каркас UI.

## Технологии

- **C# / .NET 6**
- **WinUI 3** (Windows App SDK 1.1.3)
- **MSIX** — упаковка приложения
- Поддержка x86 / x64 / arm64

## Запуск

**Требования:**
- Windows 10 версии 1809 (build 17763) или новее
- Visual Studio 2022 (17.3+) с workload «Windows application development»
- .NET 6 SDK

**Из Visual Studio:**
1. Открой `ArtGallary.sln`
2. Восстанови NuGet-пакеты
3. Выбери платформу (x64) и конфигурацию (Debug)
4. Нажми F5 для запуска

**Из CLI:**
```bash
dotnet restore
dotnet build -c Debug -p:Platform=x64
dotnet run --project ArtGallary/ArtGallary.csproj -c Debug -p:Platform=x64
```

## Структура проекта

```
ArtGallary/
├── ArtGallary.sln
└── ArtGallary/
    ├── App.xaml / App.xaml.cs       # Точка входа
    ├── MainWindow.xaml              # Главное окно (MenuBar, выбор таблиц)
    ├── ArtGallary.csproj            # WinUI 3 / .NET 6
    ├── Package.appxmanifest         # Манифест MSIX
    └── Assets/                      # Иконки, сплеш-скрин
```

## Лицензия

MIT
