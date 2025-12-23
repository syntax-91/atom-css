**https://github.com/syntax-91/atom-css**

### for use:

## vanilla.js

index.html - < link rel="stylesheet" href="./index.css">

## react

-   main.jsx - import 'g-atom-css'

**Не фреймворк. Атомарный набор примитивов.**

spacing scale:

-   sm - 4px
-   md - 8px
-   lg - 16px
-   xl - 32px
-   2xl - 64px
-   3xl - 128px
-   4xl - 256px

`:`

`g_w-fit` - with: fit;

`g_w-full` - width: full;

`g_w-screen` - width: 100vw;

`g_h-screen` - height: 100vh;

`g_m-md (y, x, ml - left, mr - right, mt - top, mb - bottom)` - margin (auto, sm, md, lg итд)

`g_p-sm (y, x, ml - left, mr - right, mt - top, mb - bottom)` - padding (auto, sm, md, lg итд)

`g_gap-sm` - gap: 4px;

`g_o-90` - opacity: 0.9;

## transition

`g_tr-bg` - transition: background-color 0.1s ease-in-out;

`g_tr-o` - transition: opacity 0.1s ease-in-out;

`g_tr-tf` - transition: transform 0.1s ease-in-out;

##

`g_radius-sm`

## border

`g_border-debug` - border 1px solid red

`g_border-white` - border 1px solid white

`g_border-black` - border 1px solid black

`g_border-gray` - border 1px solid gray

## bg

`g_bg-blur-sm`

`g_bg-debug`

`g_bg-red-100` (100, 500, 900, + green, blue, white, black, gray)

##

`g_shadow-sm`

## z-index

`g_z-90` - 0-100, absolute

## cursor

`g_cp` - cursor pointer

`g_cn` - cursor not-allowed

## container

`g_container (or g_c)` - max-width-750

## position

`g_relative, g_absolute, g_fixed` (+top,left-right,bottom)

## other

`g_disabled`,

`g_hidden`,

`g_spinner`,

`g_ovh (g_overflow)` - overflow: hidden

`g_ow-x-auto`,`g_ow-x-hidden`, `g_ow-y-auto`

## Что внутри?

✅ 0 бойлерплейта  
✅ g - префикс для изоляции (пример: "g_p-md" - padding 8px)
✅ 15kB +

**рекомендаций**

разделение ответственности:

❌ `className="myCustomClass g_p-md myCustomClass g_my-md myCustomClass"`

✅ `className={clsx("myCustomClass myCustomClass block", "g_p-md g_my-md")}`

адаптив:

`className={clsx(isMobile && "g_p-sm g_mx-lg", !isMobile && "g_p-lg")}`
