# Технические детали мода / Technical Details

## Русский

### Важно: Локализация указов категории campaigns в Stellaris 4.0+

При создании указов категории `campaigns` в Stellaris версии 4.0 и выше необходимо учитывать особенность работы локализации:

**Правило:**
- **Имя указа в коде:** без префикса "edict_"
  ```
  quick_research_1 = {
      resources = {
          category = campaigns
          ...
      }
  }
  ```

- **Ключ локализации:** с префиксом "edict_"
  ```
  l_russian:
   edict_quick_research_1:0 "Название указа"
   edict_quick_research_1_desc:0 "Описание указа"
  ```

**Почему так:** Игра автоматически добавляет префикс "edict_" при поиске локализации для указов категории campaigns.

**Пример из базовой игры:**
- Код: `fear_campaign = { ... }`
- Локализация: `edict_fear_campaign:0 "Fear Campaign"`

---

## English

### Important: Campaign Edicts Localization in Stellaris 4.0+

When creating `campaigns` category edicts in Stellaris version 4.0 and above, you need to account for a specific localization behavior:

**Rule:**
- **Edict name in code:** without "edict_" prefix
  ```
  quick_research_1 = {
      resources = {
          category = campaigns
          ...
      }
  }
  ```

- **Localization key:** with "edict_" prefix
  ```
  l_english:
   edict_quick_research_1:0 "Edict Name"
   edict_quick_research_1_desc:0 "Edict Description"
  ```

**Why:** The game engine automatically adds the "edict_" prefix when looking up localization for campaigns category edicts.

**Example from base game:**
- Code: `fear_campaign = { ... }`
- Localization: `edict_fear_campaign:0 "Fear Campaign"`
