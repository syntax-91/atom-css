for use:

# vanilla.js

index.html - < link rel="stylesheet" href="./index.css">

# react

-   main.jsx - import 'g-atom-css'

**Не фреймворк. Атомарный набор примитивов.**

## Что внутри?

✅ 0 бойлерплейта  
✅ g\_ префикс для изоляции  
✅ 13-14 kB +

Брейкпоинты:

-   sm - 4px
-   md - 8px
-   lg - 16px
-   xl - 32px
-   2xl - 64px
-   3xl - 128px
-   4xl - 256px

!!!рекомендаций

разделение ответственности:
❌ className="myCustomClass g_p-md myCustomClass g_my-md myCustomClass"

✅ className={clsx("myCustomClass myCustomClass block", "g_p-md g_my-md")}

адаптив:
✅ `className={clsx(isMobile && "g_p-sm g_mx-lg", !isMobile && "g_p-lg")}`
