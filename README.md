# Email HTML Template & Rules

### Полезные сервисы

| Сайт                           | Ссылка                                                       |
| ------------------------------ | ------------------------------------------------------------ |
| Validator 1                    | https://validator.w3.org/                                    |
| Validator 2                    | https://htmlemailcheck.com/                                  |
| Проверка кроссплатформености 1 | https://caniemail.com/                                       |
| Проверка кроссплатформености 2 | https://caniuse.email/                                       |
| CSS Inliner 1                  | https://putsmail.com/inliner                                 |
| CSS Inliner 2                  | https://www.campaignmonitor.com/resources/tools/css-inliner/ |
| Test Email                     | https://putsmail.com/                                        |
| Test Email (Devices Emulator)  | https://www.emailonacid.com/                                 |

### Правила

- Общие
  - DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN"
  - Проверять валидность
  - Использовать inline-стиоли
  - Только табличная верстка
  - Избегать излишних вложенностей (таблица в таблице и тд.)
  - Можно использовать картинки вместо кнопок
  - Писать стили полностью (color: #fffff, padding-top: 12px padding-left :12px...)
  - Желательно использовать безопасные шрифты — https://websitesetup.org/web-safe-fonts-html-css/
  - Использовать — valign, align
  - Всегда cellpadding, cellspacing, border = 0
  - Переносы только через <br />
  - Использовать только px (не использовать rem, em)
  - Использовать прехедер — <div style="font-size:0px;font-color:#ffffff;opacity:0;visibility:hidden;width:0;height:0;display:none;">текст прехедера</div>
  - Всегда использовать цвет фона для любой картинки (прим.: bgcolor="#ffffff")
  - Использовать резиновую верстку или две версий — пк, моб
  - Особое внимание атрибутам "title" у ссылок, "alt" у картинок
  - Можно использовать фреймвор — [mjml.](https://mjml.io/) (outlook?)
  - Не испрользовать стили — box-shadow, @font-face, iframe, picture, video
  - Не использовать — flex, grid
  - Мобильная версия до 599px
  - Картинки должны быть x2 от нужного размера (Retina, High DPI)
  - Не поддерживается JavaScript (можно использовать utm-метки для отслеживания переходов)
  - Использовать только графику форматов — .jpg, .png, .gif? (не использовать base64, .svg, .webp...)
  - Не использовать пустые ячейки для отступов (использовать padding, border у th/td)
  - Размер письма не более 1 Мб
- Outlook
  - Можно использовать спец коментарии для outlook <!--[if mso | EI]> Code here <!--[endif]-->
  - Не поддерживается background-image
  - Сложности с .gif и анимацией (подобрать подход)
  - Картинки загружаются только после клика внутри письма
  - Не работают @media-запросы (можно делать отдельную версия без @media-запросов)
- Google
  - Не прывышать 102 Кб кода письма (картинки не учитываются)
