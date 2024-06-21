@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@500&display=swap");
@import url("https://eject37.github.io/DiscordTheme/HideTrash.css");
@import url("https://eject37.github.io/DiscordTheme/ScrollBar.css");
@import url("https://eject37.github.io/DiscordTheme/RoundUserPanel.css");
@import url("https://eject37.github.io/DiscordTheme/OldMicrophone.css");
@import url("https://eject37.github.io/DiscordTheme/ChangeSearchBarToIcon.css");
@import url("https://eject37.github.io/DiscordTheme/RegionFlags.css");

:root {
    --app-bg: url(https://i.giphy.com/9JxkPTP3alOykb8PmQ.webp);
    --blur-bg: 80px;
    --brightness-bg: 0.35;
    --border-main: 1px solid rgba(255, 255, 255, 0.1);
}

.theme-dark {
    /* Border в чате на сообщениях где код */
    --background-secondary-alt: rgba(255, 255, 255, 0.05);
    --background-tertiary: var(--background-secondary-alt);
    /* Бейджики  уведомлений */
    --status-danger: rgba(202, 90, 99, 0.9);
    /* ссылки*/
    --text-link: rgb(125, 170, 233);
    /* много где */
    --background-primary: rgba(245, 245, 245, 0.1);
    /* много где используется*/
    --background-secondary: rgba(255, 255, 255, 0.05);
    /* загруска сообщений в чате*/
    --bg-overlay-chat: rgba(255, 255, 255, 0.05);
    /* контекстное меню КРАСНАЯ кнопкА при наведении */
    --button-danger-background: rgba(250, 100, 135, 0.25);
    /* наводишься там где мьют микро слева снизу */
    --background-modifier-selected: rgba(190, 190, 190, 0.25);
    --background-floating: rgba(190, 190, 190, 0.25);
    --status-positive-background: rgba(190, 190, 190, 0.25);
}
:root {
    /* Шрифт */
    --font-primary: "Montserrat", Arial, sans-serif;
    --font-display: "Montserrat", Arial, sans-serif;
    --font-headline: "Montserrat", Arial, sans-serif;

    --status-positive: rgba(255, 255, 255, 0.7);
    --text-positive: rgba(255, 255, 255, 0.67);
    /* Цвет загрузки демок и прочего */
    --primary-700: rgba(200, 200, 200, 0.1);
    /* bar */
    --brand-500: rgb(100, 100, 100);
    /* Бордер чекбоксов, спиннер */
    --brand-400: rgba(170, 170, 170, 0.4);
    /* текст какой то */
    --brand-560: rgb(220, 220, 220);
    /* контекстное меню кнопки при наведении */
    --brand-530: rgba(230, 240, 255, 0.15);
    /* контекстное меню когда зажал */
    --brand-600: rgba(255, 255, 255, 0.3);
    /* мьют микро */
    --red-400: rgba(202, 90, 116, 0.7);
    /* стрелочка наводишься там где вайфай  */
    --green-360: rgba(230, 240, 255, 0.15);
    /* задний цвет там где сервер выбираешь */
    --primary-630: rgba(230, 240, 255, 0.15);
    /* можно выключить микрофон */
    --primary-860: rgba(202, 90, 99, 0.9);
    /* мьют микро на панели снизу слева */
    --important-messages-color: #fdbdbd;
    /* Длина и отступ панели табов в настройках */
    --custom-standard-sidebar-view-sidebar-content-width: 217px;
    --custom-standard-sidebar-view-standard-padding: 100px;
}

/* Шрифт */
:root:lang(bg),
:root:lang(el),
:root:lang(ru),
:root:lang(uk) {
    --font-primary: "Montserrat", Arial, sans-serif;
    --font-display: "Montserrat", Arial, sans-serif;
    --font-headline: "Montserrat", Arial, sans-serif;
}

/* гифка для всего дс */
body {
    background: var(--app-bg) no-repeat;
    background-position: 15%;
    background-size: 105% 105%;
}

/* добавляет блюр и затемнение на задний фон */
.bg_d4b6c5 {
    backdrop-filter: blur(var(--blur-bg)) brightness(var(--brightness-bg));
}

/* Credits */
.info_c5a741::before {
    content: "Theme by Eben Gemink";
    color: var(--text-muted);
    font-size: 14px;
    padding-bottom: 10px;
    display: block;
}

/* убирает задний цвет для гифки */
.chatContent_a7d72e,
.chat_a7d72e,
.sidebar_a4d4d9,
.panel_bf1a22,
.container_adcaac,
.container_b2ca13,
.wrapper_fea3ef,
.callContainer_d880dc,
.wrapper_d880dc,
.panels_a4d4d9,
.privateChannels_f0963d,
.scroller_c47fa9,
.themedBackground_d0696b,
.themed_e44302,
.bg_d4b6c5,
#app-mount,
.app_a01fb1,
.codeView_ad9cbd.hljs,
.menu_d90b3d:not(.menu_ad5fac),
.embedFull_ad0b71,
.container_cbd271,
.members_cbd271,
.container_ee69e0,
.member_cbd271,
.sidebarRegionScroller_c25c6d,
.standardSidebarView_c25c6d,
.layer_d4b6c5,
.contentRegionScroller_c25c6d,
.contentRegion_c25c6d,
.container_c2739c,
.nowPlayingColumn_c2739c,
.container_bf550a,
.inset_c0f6a6,
.attachedBars_d0696b,
.background_b69b77,
.fieldList_b69b77,
.premiumBackground_c6d722,
.overlayBackground_c69a7b,
.bannerNormal_ab876d,
.userProfileInnerThemedNonPremium_c69a7b,
.container_f1fd9c,
.header_f1fd9cm,
.mediaBarInteractionVolume_f7877e,
.medium_f9a4c9,
.modal_f31a4d,
.authBoxExpanded_dc6abe {
    background: transparent !important;
}

/* фиксит 4px title bar */
.withFrame_a934d8 {
    margin-top: 0;
    padding-top: 4px;
}

/* убирает залупу */
.form_a7d72e:before, /*градиент возле чатбокса*/
.form_a7d72e:after,
.children_e44302:after,/* какой то градиент сверху хз */
.protip_f4e139, /* нахуй оно надо (в найти или начать беседу) */ 
.block_dcc874, /* нахуй оно надо (в закрепах) */
.tutorial_c36bbe.shown_c36bbe, /* нахуй оно надо (подсказка в найти или начать беседу) */
.userSettingsSecurityImage_ad4a7c,
.ready_e40c16, /* нахуй оно надо (моя учетная запись)*/ 
.content_a7d72e:before,
.container_da1432 /* черная полосаааа*/ {
    display: none !important;
}

/* Выделение текста */
::selection {
    background: rgba(94, 98, 106, 0.4) !important;
}

/* Кнопки в голосовом чате (офф микро, дать демку, выйти из звонка) */
#app-mount .staticButton_ef18ee,
#app-mount .contextMenuNub_ef18ee {
    background-color: rgba(255, 255, 255, 0.1) !important; /*off call*/
    color: rgb(255, 255, 255) !important;
}
#app-mount .staticButton_ef18ee:hover {
    background-color: rgba(255, 255, 255, 0.2) !important; /*off call*/
}

/* демка */
.callContainer_d880dc {
    background: linear-gradient(
        rgba(0, 0, 0, 0.15),
        rgb(0, 0, 0, 0.1)
    ) !important;
    box-shadow: inset 0 0 10px rgba(100, 100, 100, 0.1);
    border-radius: 10px;
    border: var(--border-main);
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 10px;
}
/* фикс демки в полном экране */
.callContainer_d880dc:has(.actionRow_f8a4f3) {
    margin: 0;
    border-radius: 0;
    border: none;
    box-shadow: none;
}

/* меняет градиент при навидиении там где демка */
.gradientContainer_dd069c {
    background-image: linear-gradient(
        rgba(255, 255, 255, 0.04) 0%,
        rgba(0, 0, 0, 0) 50%
    );
}

/* ввод сообщений (chatbox) */
.channelTextArea_a7d72e {
    background: rgba(255, 255, 255, 0.03) !important;
    border: var(--border-main);
    border-radius: 15px;
    box-shadow: inset 0 0 5px rgba(100, 100, 100, 0.2);
}
.scrollerSpacer_e2e187 {
    height: 25px;
}
.form_a7d72e {
    margin-top: 0;
}

/* Пользователи слева в списке, справа на серверах, каналы на серверах */
.interactive_f5eb4b,
.member_cbd271,
.layout_e9f61e,
.modeSelected_d8bfb3 .link_d8bfb3,
.wrapper_d8bfb3 .link_d8bfb3 {
    transition: 0.1s;
    margin-left: 5px;
    width: 95%;
    border-radius: 10px;
}
.selected_f5eb4b,
.interactive_f5eb4b:hover,
.member_cbd271:hover,
.modeSelected_d8bfb3 .link_d8bfb3,
.modeSelected_d8bfb3:hover .link_d8bfb3 {
    background: linear-gradient(
        rgba(184, 184, 184, 0.225),
        rgba(255, 255, 255, 0.144)
    );
    margin-left: 7px;
}
.modeSelected_d8bfb3 .link_d8bfb3,
.wrapper_d8bfb3 .link_d8bfb3 {
    transition: none;
}

/* Строка поиска слева сверху */
.searchBarComponent_f0963d {
    margin-left: 7px;
    width: 94% !important;
}

/* Стеклеянные окна */
.searchBarComponent_f0963d, /* Строка поиска слева сверху */
.menu_d90b3d:not(.menu_ad5fac) /* Контекстное меню */ {
    background: rgba(255, 255, 255, 0.03) !important;
    box-shadow: inset 0 0 10px rgba(100, 100, 100, 0.25) !important;
    border-radius: 10px !important;
}

/* Контекстное меню Blur */
.menu_d90b3d:not(.menu_ad5fac):before {
    position: absolute;
    content: " ";
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    backdrop-filter: blur(20px);
    pointer-events: none;
    z-index: -1;
}
/* фикс когда открыта картинка */
#image-context[class*="menu_d90b3d"] {
    backdrop-filter: blur(15px) brightness(var(--brightness-bg));
}
.menu_d90b3d:not(.menu_ad5fac) .submenu_d90b3d:before {
    width: calc(100% - 16px);
    left: 8px;
}

/* панель пользователя */
[class^="sidebar_"] [class^="panels_"] {
    box-shadow: 0 0 3px 1px rgba(0, 0, 0, 0.45),
        inset 0 0 10px rgba(100, 100, 100, 0.2);
}
[class^="sidebar_"] [class^="panels_"] [class^="container_"],
[class^="sidebar_"] [class^="panels_"] [class^="panel_"] {
    background-color: rgba(100, 100, 100, 0.04) !important;
}

/* Загружаемые файлы и разные фоны в сообщениях */
.attachment_a4623d.newMosaicStyle_a4623d,
.newMosaicStyle_ad9cbd .codeView_ad9cbd,
.newMosaicStyle_ad9cbd .footer_ad9cbd,
.newMosaicStyle_ad9cbd .textContainer_ad9cbd,
.grid_ad0b71,
.wrapper_b9fe76,
.markup_d6076c code,
.content_fc5f50 {
    background: rgba(100, 100, 100, 0.15);
}

/* При наведении в чате на сообщение справа тул панель с действиями */
.wrapper_ef319f {
    border-radius: 10px;
    border: 1px solid var(--background-secondary-alt);
    backdrop-filter: blur(10px);
    background: rgba(165, 165, 165, 0.15);
}

/* Сверху слева иконка дискорда, убираем цвет если не активна */
.childWrapperNoHoverBg_f90abb {
    background: transparent;
}

/* Ссылки в чате */
a.anchor_af404b > span:not(.username_de3235) {
    background: linear-gradient(
        90deg,
        rgb(78, 208, 255),
        rgb(230, 98, 230),
        rgb(171, 189, 56)
    );
    color: transparent;
    background-clip: text;
}

/* друзья */
/* друзья */
/* друзья */
/* друзья */
/* друзья */
/* друзья */
.wrapper_cd82a7,
.section_cd82a7 {
    background: rgba(100, 100, 100, 0.15);
}
.outer_c0f6a6.interactive_c0f6a6:hover,
.theme-dark .outer_c0f6a6.active_c0f6a6 {
    background: rgba(100, 100, 100, 0.3) !important;
}
.actionButton_e01b91 {
    background: rgba(100, 100, 100, 0.3) !important;
}
/* друзья */
/* друзья */
/* друзья */
/* друзья */
/* друзья */
/* друзья */

/* поиск нажатие */
.quickswitcher_f4e139 {
    background: rgba(100, 100, 100, 0.15);
    box-shadow: inset 0 0 15px rgba(255, 255, 255, 0.1);
    padding: 3%;
    padding-right: 34px;
    backdrop-filter: blur(10px);
}
.input_f4e139 {
    background: rgba(100, 100, 100, 0.1);
    width: 103.4%;
}
.scroller_f4e139 {
    background: rgba(100, 100, 100, 0.15);
}

/* Если тебя упомянули */
.mentioned_d5deea {
    background: rgba(226, 226, 226, 0.08) !important;
}
/* Линия слева в сообщении в котором тебя упомянули */
.mentioned_d5deea:before {
    background-color: rgba(226, 226, 226, 0.16);
}

/* теги когда тэгаешь кого то */
.autocomplete_f23da8 {
    background-color: rgba(35, 35, 35, 0.2) !important;
    backdrop-filter: blur(15px);
    border-radius: 10px;
    border: 1px solid var(--background-secondary-alt);
}

/* ответить , вы просматриваете старые сообщения*/
.replyBar_b11c5e,
.jumpToPresentBar_cf58b5 {
    background: rgba(100, 100, 100, 0.07);
    border-bottom: 1px solid rgba(228, 228, 228, 0.03);
}
.jumpToPresentBar_cf58b5 {
    backdrop-filter: blur(20px);
    border-radius: 10px;
    border: 1px solid var(--background-secondary-alt);
}

/* авторизованные пользователи */
.cardPrimary_a298b8 {
    background: rgba(100, 100, 100, 0.07);
}
/* семейный центр */
.container_b01337,
.container_d00e26,
.container_a2e886 {
    background: rgba(100, 100, 100, 0.1);
    border: 1px solid var(--background-secondary-alt);
}

/* Настройки > Профили > Попробуйте нитро */
.premiumFeatureBorder_c6d722 {
    background: rgba(100, 100, 100, 0.15) !important;
    border: 1px solid var(--background-secondary-alt);
}

/* textbox */
.input_f8bc55,
.input_f8bc55:hover {
    background: rgba(100, 100, 100, 0.2) !important;
    border: 1px solid var(--background-secondary-alt);
}
.input_f8bc55.focused_f8bc55,
.input_f8bc55:focus {
    border: 1px solid rgba(255, 255, 255, 0.15);
}
/* Настройки > Профили > Обо мне (textbox) */
.bioTextArea_ccf27d {
    background: rgba(100, 100, 100, 0.2) !important;
    border: var(--border-main);
}

/* предпросмотр профиля */
.userProfileInnerThemedNonPremium_c69a7b {
    border: var(--border-main);
}

/* SelectBox (Настройки > Конфиденциальность) */
.lookFilled_f6639d.select_f6639d {
    background: rgba(100, 100, 100, 0.2) !important;
    border: var(--border-main);
}
/* open select box  */
.popout_f6639d {
    background: rgba(100, 100, 100, 0.2) !important;
    backdrop-filter: blur(20px);
    border: var(--border-main);
}
/* Width fix  */
.popout_f6639d.scrollerBase_c49869 {
    overflow: auto !important;
}

/* фильтр спама */
.itemFilled_eb92a8 {
    background: rgba(100, 100, 100, 0.2) !important;
}

/* Toogle ON */
.container_cebd1c.checked_cebd1c {
    background-color: rgba(255, 255, 255, 0.4) !important;
}
/* Toogle OFF */
.container_cebd1c {
    background-color: rgba(100, 100, 100, 0.4) !important;
}

/* Настройки > Самая нижняя панель */
.card_a298b8:not(.outline_a298b8) {
    background-color: rgba(100, 100, 100, 0.15) !important;
}

/* интеграция */
.connection_e2a436,
.accountButtonInner_e2a436,
.accountBtnInner_ec99f9 {
    background-color: rgba(100, 100, 100, 0.2) !important;
}

/* WARNING (Настройки > Горячие клавиши) */
.vc-backup-restore-card,
.warning_f20685 {
    border: 1px solid rgba(240, 230, 100, 0.4);
}

/* Настройки > Зарегистрированные игры (верхняя панель)  */
.notDetected_fd966d {
    background-color: rgba(100, 100, 100, 0.1) !important;
    border: var(--border-main);
}

/* Blue + Red Buttons */
button[class*="lookFilled_dd4f85"] {
    background-color: rgba(150, 150, 150, 0.25) !important;
    border-radius: 7px;
}
button[class*="lookFilled_dd4f85"]:hover {
    background-color: rgba(150, 150, 150, 0.35) !important;
}
/* Кнопка деавторизировать */
.lookOutlined_dd4f85.colorRed_dd4f85 {
    border: var(--border-main);
}
.lookOutlined_dd4f85.colorRed_dd4f85:hover {
    background-color: rgba(190, 30, 60, 0.3);
    border: 1px solid rgba(190, 30, 60, 0.4);
}

/* MessageBox`ы  */
.container_acae5d.root_f9a4c9,
.modalSize_e1cc86.root_f9a4c9,
.small_f9a4c9,
.medium_f9a4c9 {
    background-color: rgba(100, 100, 100, 0.2) !important;
    backdrop-filter: blur(25px);
    border-radius: 10px;
}
.footer_f9a4c9,
.message_ddcc45 {
    background-color: rgba(100, 100, 100, 0.1) !important;
    border-radius: 10px;
}

/* Настройки > Левая панель (табы) */
.side_a0 .selected_a0 {
    background-color: rgba(100, 100, 100, 0.3) !important;
}
.side_a0 .item_a0 {
    border-radius: 10px;
}

/* Закрепленные сообщения */
.messagesPopoutWrap_ac90a2,
.container_eedf95 {
    background-color: rgba(100, 100, 100, 0.1) !important;
    backdrop-filter: blur(35px);
}
.messageGroupWrapper_ac90a2 {
    background-color: rgba(100, 100, 100, 0.1) !important;
}
.messagesPopoutWrap_ac90a2 {
    margin-top: -15px; /* Фикс для margin области разговора (демки) что бы дискорд не прыгал */
}

/* Открытый поиск в диалоге (когда уже просматриваешь найденные сообщения) */
.searchResultsWrap_c2b47d {
    background-color: rgba(100, 100, 100, 0.2) !important;
}
.searchResult_ddc613 {
    background-color: rgba(100, 100, 100, 0.1) !important;
    border: var(--border-main);
}

/* Кнопка + (Добавить сервер) */
.circleIconButton_db6521 {
    background-color: rgba(200, 205, 210, 0.1) !important;
    color: rgba(200, 200, 200, 0.8) !important;
}

/* Поиск в чате справа сверху при наведении */
.searchBar_a46bef:hover,
.focused_a46bef .searchBar_a46bef,
.open_a46bef .searchBar_a46bef {
    background-color: rgba(100, 100, 100, 0.25);
    backdrop-filter: blur(20px);
}

/* кнопка пригласить на сервер друга */
.inviteRowButton_cedfaf,
.lookOutlined_dd4f85.colorGreen_dd4f85:hover {
    background-color: rgba(100, 100, 100, 0.25);
    border: var(--border-main) !important;
    width: 110px;
    border-radius: 6px;
}

/* когда кто то пиздит */
.border_ba4b17.speaking_ba4b17,
.border_a5cd29.speaking_a5cd29,
.speaking-3K28iH,
.speaking_fb2f1c,
.avatarSpeaking_c51b4e {
    box-shadow: inset 0 0 10px rgb(130, 130, 130);
}

/* устройстав задний цвет */
.sessionIcon_c7a2c0,
.legacySession_c7a2c0 .sessionIcon_c7a2c0 {
    filter: invert();
    background-color: rgba(100, 100, 100, 0.25) !important;
}

/* BETA где то в настройках */
.textBadge_f05120 {
    background-color: rgba(100, 100, 100, 0.5) !important;
}

/* ссылки при клике которые не обычные ссылки */
.fileNameLink_a4623d,
.link_f0135d,
.lookLink_dd4f85 {
    background: linear-gradient(90deg, rgb(255, 84, 132), rgb(137, 90, 255));
    color: transparent;
    background-clip: text;
}

/* ToolTip */
.tooltipPrimary_b6c360,
.tooltipGreen_b6c360 {
    background-color: rgba(100, 100, 100, 0.2) !important;
    backdrop-filter: blur(10px);
    border-radius: 10px;
}

/* цвет профиля когда тыкаешь сверху */
.popoutBanner_c3e427,
.banner_c3e427.modalBanner_c3e427 {
    background-color: rgba(100, 100, 100, 0.2) !important;
}
.userPopoutInner_c69a7b:before {
    position: absolute;
    content: " ";
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    backdrop-filter: blur(20px);
    pointer-events: none;
    z-index: -1;
}

/* идет загрузка файла */
.attachment_a4623d {
    background-color: rgba(100, 100, 100, 0.1) !important;
}
/* вставка файла в чат */
.upload_df1eaf {
    background-color: rgba(100, 100, 100, 0.2) !important;
    border-radius: 10px;
}
/* Green Ico demka ON */
.upperBadge_c5f96a > .iconBadge_c96c45 {
    background-color: transparent !important;
    background-color: rgb(71, 71, 71) !important;
}

/* Шрифт для плагина который показывает сколько времени я в голосовом канале */
.text-xs-normal__46d75 span {
    font-family: var(--font-primary) !important;
}

/* шрифт ГОЛОСОВАЯ СВЯЗЬ ПОДКЛЮЧЕНА */
.contents_dd4f85 {
    font-weight: 500;
}

/* ачивмент в профиле */
.profileBadges_f89da9 {
    background-color: rgba(140, 140, 140, 0.2) !important;
}

/* квадрат загрузки */
.loadingPopout_a8c724 {
    border-radius: 10px;
}
.container_e40c16.fixClipping_c7e9c6 {
    backdrop-filter: blur(30px);
}
/* сверху в чате новые сообщения */
.newMessagesBar_cf58b5 {
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(10px);
    border: var(--border-main);
}

/* форумы на сервере */
.mainCard_a6d69a {
    background: rgba(255, 255, 255, 0.1);
}
.container_d331f1:hover {
    background: rgba(255, 255, 255, 0.2);
}

/* сообщение при входе в D$ */
.tip_e40c16 {
    color: transparent;
    max-width: 1000px !important;
}
.tip_e40c16::before {
    animation-duration: 1s;
    animation-name: slidein;
    content: "Theme created by Eben Gemink";
    color: white !important;
    display: flex;
    justify-content: center;
}
@keyframes slidein {
    from {
        opacity: 0;
    }

    to {
        opacity: 1;
    }
}

/* дискорд прокрутка при загрузке */
.scroller_c6b11b,
.thin_c49869.scrollerBase_c49869.fade_c49869,
.brand_a0 {
    background: transparent !important;
}

/* чат ?????? */
.chat_a7d72e.content_a7d72e.container_f1fd9c {
    background: rgba(255, 0, 0, 1) !important;
}

/* просмотр каналов на сервере */
.channelRow_f04d06 {
    background: rgba(255, 255, 255, 0.1) !important;
}

/* в вашем списке каналов нет этого канала НА СЕРВЕРЕ  */
.chatHeaderBar_efb691 {
    background: rgba(255, 255, 255, 0.1) !important;
}

/* ПОМЕТКА БОТА БОТ */
.botTagRegular_a02df3 {
    background: rgba(255, 255, 255, 0.15) !important;
}

/* прN наведении на упоминание */
.interactive:hover {
    background: rgba(255, 255, 255, 0.15) !important;
}

/* Поставленная реакция на сообщение */
.reactionMe_ec6b19 {
    background: rgba(255, 255, 255, 0.15) !important;
}

/* ветки на серверах */
.container_e664f3 {
    backdrop-filter: blur(25px);
}

/* Иконка дискорда слева сверху */
.wrapper_f90abb:hover .childWrapper_f90abb,
.wrapper_f90abb.selected_f90abb .childWrapper_f90abb {
    background: rgba(255, 255, 255, 0.1) !important;
    box-shadow: inset 0 0 10px rgba(255, 255, 255, 0.1) !important;
}

/* Кнопки в контекстном меню */
.colorDefault_d90b3d.focused_d90b3d {
    border-radius: 10px;
}

/* удалить сообщение в контекстом меню */
.colorDanger_d90b3d {
    color: rgb(202, 90, 116);
}

/* способы скама на нитро на маманта */
.paymentPane_f66684,
.paginator_f66684,
.payment_a28a08 {
    background: rgba(255, 255, 255, 0.015) !important;
}

/* панель эмодзи */
.contentWrapper_af5dbb {
    backdrop-filter: blur(20px);
}
.popoutContainer_cf58b5 {
    background: rgba(255, 255, 255, 0.05) !important;
}

/* бляр на баре  */
.tooltipGrey_b6c360 {
    backdrop-filter: blur(10px);
}

/* выбор контекстого меню галочки фон */
.colorDefault_d90b3d.focused_d90b3d path {
    fill: rgba(255, 255, 255, 0.3);
}

/* фон выбора сервера  */
.regionSelectPopout_ccb5ca {
    backdrop-filter: blur(15px);
    border-radius: 10px;
    background: rgba(255, 255, 255, 0.1) !important;
    border: var(--border-main);
}

/* добавить в друзья главный экран */
.tabBar_c2739c .addFriend_c2739c.addFriend_c2739c.addFriend_c2739c:hover {
    background: rgba(255, 255, 255, 0.25) !important;
}

/* добавить в друзья бордер */
.addFriendInputWrapper_de812f:focus-within {
    border: var(--border-main);
}

/* сведение 0 сервере */
.container__13b2a {
    backdrop-filter: blur(20px);
    border-radius: 10px;
    border: var(--border-main);
}

/* зажатие на удалить сообщения */
.colorDanger_d90b3d:active:not(.hideInteraction_d90b3d) {
    background: rgba(202, 90, 116, 0.6) !important;
}
/* фикс бордера в контекстном меню при зажатии и отведении */
.colorDefault_d90b3d:active:not(.hideInteraction_d90b3d) {
    border-radius: 10px;
}

/* плагин membercount */
.vc-membercount-widget {
    --color-online: rgba(108, 255, 223, 0.7);
}

/* смотреть  стрим */
.streamPreview_ba4b17 {
    background: transparent !important;
}
.streamPreview_ba4b17 button {
    backdrop-filter: blur(10px);
}

/* когда демку можно включить */
.colorable_ef18ee.primaryDark_ef18ee .centerIcon_ef18ee {
    color: rgb(255, 255, 255);
}

/* можно выключить демку */
.colorable_ef18ee.white_ef18ee,
.colorable_ef18ee.white_ef18ee .centerIcon_ef18ee {
    color: rgba(202, 90, 99, 0.9);
}

/* линия под ссылками */
.anchor_af404b {
    text-decoration-color: rgba(255, 255, 255, 0.45) !important;
}

/* Черная линия в чате в разговоре */
.resizeHandle_c0a559 {
    background-color: transparent;
}

/* Уведомление о обновлении VenCord */
.vc-notification {
    backdrop-filter: blur(20px);
}

/* фон сообщений при наведении */
.message_d5deea:hover {
    background: rgba(190, 190, 190, 0.03) !important;
}

.popout__4c91, /* статус действий на сервере	 */ 
.reactionTooltip_fba897  /* наведение на реакцию */ {
    backdrop-filter: blur(15px);
}

/* добавить учетную запись */
.authBoxExpanded_dc6abe,
.modal_f31a4d {
    background: rgba(255, 255, 255, 0.05) !important;
    backdrop-filter: blur(15px);
}

/* Add server */
.circleIconButton_db6521:hover > .circleIcon_db6521 {
    animation-name: ani-rotate;
    animation-duration: 1s;
}
/* статистика пинга  */
.debugPanelStandalone_feab95 {
    backdrop-filter: blur(15px);
    border-radius: 15px;
}

/* верхний цвет откртия профиля */
.settingsBanner_c3e427 {
    background-color: rgba(100, 100, 100, 0.2) !important;
}
/* полоска за которую перетягиваешь звук */
.grabber_c7a159 {
    background-color: rgba(255, 255, 255, 0.5) !important;
    border: var(--border-main);
}
/* выбор звуков пердежа */
.picker_cd703d {
    backdrop-filter: blur(15px) !important;
}
/* Настройки > склад подарков */
.giftCardButton_d8f41e {
    background-color: rgba(100, 100, 100, 0.2) !important;
    border: var(--border-main) !important;
}
.giftCardButton_d8f41e:hover {
    background-color: rgba(100, 100, 100, 0.4) !important;
}

@keyframes ani-rotate {
    0% {
        transform: rotate(0);
    }
    100% {
        transform: rotate(360deg);
    }
}
