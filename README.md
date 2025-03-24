# CherryStudio-Aero

English | [简体中文](README-cmn_CN.md) | [繁體中文](README-cmn_TW.md) | [廣東話](README-jyut.md)

> [Aero: **A**uthentic, **E**nergetic, **R**eflective and **O**pen](https://en.wikipedia.org/wiki/Windows_Aero)

Give your [Cherry Studio](https://github.com/CherryHQ/cherry-studio) a modern, Aero theme

> [!NOTE]
> Frosted glass effect only works on Cherry Studio for macOS.

## Screenshots

![image](https://github.com/user-attachments/assets/f1b45077-49e7-4c04-8c5f-b5099d1020aa)
![image](https://github.com/user-attachments/assets/a1203c88-9efa-489b-b3e7-a5f41961fd9e)
![image](https://github.com/user-attachments/assets/86315ef8-9bdc-4525-a4cb-b143f8608414)
![image](https://github.com/user-attachments/assets/76d6ffdd-a6be-4694-98b8-69a788208b80)

## Getting started

Copy the following CSS to `Settings` -> `Display Settings` -> `Custom CSS`

![image](https://github.com/user-attachments/assets/a8e595fb-d093-4972-b439-6dfb9029c9ae)

CSS

```css
/* Cherry Studio Aero Theme */
/* https://github.com/hakadao/CherryStudio-Aero */

body[theme-mode=light] {
  --fill-1: rgba(120 120 122 / 0.1);
  --fill-2: rgba(120 120 122 / 0.15);
  --fill-3: rgba(120 120 122 / 0.20);

  --color-white: var(--fill-1);
  --color-white-soft: var(--fill-2);
  --color-white-mute: var(--fill-3);
}

:root {
  --fill-1: rgba(120 120 122 / 0.15);
  --fill-2: rgba(120 120 122 / 0.20);
  --fill-3: rgba(120 120 122 / 0.25);

  --color-black: var(--fill-1);
  --color-black-soft: var(--fill-2);
  --color-black-mute: var(--fill-3);
}

@media (prefers-color-scheme: dark) {
  body[theme-mode=light] {
      background: rgba(255 255 255 / 0.3);
  }
}

@media (prefers-color-scheme: light) {
  body[theme-mode=dark] {
      background: rgba(0 0 0 / 0.2);
  }
}

[theme-mode=light] #content-container,
[theme-mode=light] .minapp-drawer .ant-drawer-body {
  background-color: rgba(120 120 122 / 0.05);
}

[theme-mode=dark] #content-container,
[theme-mode=dark] .minapp-drawer .ant-drawer-body {
  background-color: rgba(120 120 122 / 0.05);
}

.home-tabs,
[class^=ProgramSection],
[class^=IconSection],
#messages {
  background-color: transparent;
}

[class^=TopicListItem] .menu {
  background-color: transparent !important;
}

#inputbar,
.system-prompt {
  background-color: var(--fill-1);
}

[theme-mode=light] #chat,
[theme-mode=light] [class^=SettingGroup],
[theme-mode=light] [class^=MainContainer],
[theme-mode=light] [class^=MainContent] {
  background-color: hsla(0 0% 100% / 0.4);
}

[theme-mode=dark] #chat,
[theme-mode=dark] [class^=SettingGroup],
[theme-mode=dark] [class^=MainContainer],
[theme-mode=dark] [class^=MainContent] {
  background-color: hsla(0 0% 0% / 0.2);
}

[theme-mode=light] [class^=ant-modal],
[theme-mode=light] #root[style*="background: var(--color-white)"] {
  --color-white: #ffffff;
  --color-white-soft: #f2f2f2;
  --color-white-mute: #eee;

  --color-background: var(--color-white);
  --color-background-soft: var(--color-white-soft);
  --color-background-mute: var(--color-white-mute);
}

[theme-mode=dark] [class^=ant-modal] {
  --color-black: #1b1b1f;
  --color-black-soft: #262626;
  --color-black-mute: #363636;

  --color-background: var(--color-black);
  --color-background-soft: var(--color-black-soft);
  --color-background-mute: var(--color-black-mute);
}

.bubble .message-user,
[class^=ant] {
  --color-black: #1b1b1f;
  --color-black-soft: #262626;
  --color-black-mute: #363636;
  --color-white: #ffffff;
  --color-white-soft: #f2f2f2;
  --color-white-mute: #eee;

  --chat-text-user: var(--color-black);
}
```
