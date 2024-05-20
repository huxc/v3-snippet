# v3-snippets

## VS Code vue3、JS(ES6) snippets

---

[![Version](https://vsmarketplacebadge.apphb.com/version/xabikos.JavaScriptSnippets.svg)](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/xabikos.JavaScriptSnippets.svg)](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets)
[![Ratings](https://vsmarketplacebadge.apphb.com/rating/xabikos.JavaScriptSnippets.svg)](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets)

This extension contains code snippets for JavaScript in ES6 syntax for [Vs Code][code] editor (supports both JavaScript and TypeScript).

### Note

**All the snippets include the final semicolon `;` There is a fork of those snippets [here](https://marketplace.visualstudio.com/items?itemName=jmsv.JavaScriptSnippetsStandard)
made by @jmsv where semicolons are not included. So feel free to use them according to your needs.**

## Sponsors

<p><a title="Try CodeStream" href="https://sponsorlink.codestream.com/?utm_source=vscmarket&amp;utm_campaign=jses6codesnippets&amp;utm_medium=banner"><img src="https://alt-images.codestream.com/codestream_logo_jses6codesnippets.png"></a></br>
Request and perform code reviews from inside your IDE.  Review any code, even if it's a work-in-progress that hasn't been committed yet, and use jump-to-definition, your favorite keybindings, and other IDE tools.<br> <a title="Try CodeStream" href="https://sponsorlink.codestream.com/?utm_source=vscmarket&amp;utm_campaign=jses6codesnippets&amp;utm_medium=banner">Try it free</a></p>

## Installation

In order to install an extension you need to launch the Command Palette (Ctrl + Shift + P or Cmd + Shift + P) and type Extensions.
There you have either the option to show the already installed snippets or install new ones. Search for _JavaScript (ES6) code snippets_ and install it.

## Supported languages (file extensions)

- JavaScript (.js)
- Vue (.vue)

## Snippets

Below is a list of all available snippets and the 关键词 s of each one. The **⇥** means the `TAB` key.

### vue3

|    关键词     |                                                                       代码片段                                                                        |
| :-----------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: |
|  `v3Setup→`   | `<template><div></div></template><script setup>const props = defineProps({});const emits = defineEmits();</script><style scoped lang="scss"></style>` |
| `v3Options→`  |                               `<template><div></div></template><script>...</script><style lang="scss" scoped></style>`                                |
|    `vref→`    |                                                                `const ref = ref(xxx);`                                                                |
|   `vproxy→`   |                                                       `const { proxy } = getCurrentInstance()`                                                        |
|   `vwatch→`   |                                               `watch(xx, (newValue, oldValue) => {}, { deep: true });`                                                |
| `vcomputed→`  |                                                            `const $1 = computed(() => {})`                                                            |
| `vnextTick→`  |                                                                 `nextTick(() => {})`                                                                  |
| `vonMounted→` |                                                                 `onMounted(() => {})`                                                                 |
| `vonUpdated→` |                                                                 `onUpdated(() => {})`                                                                 |
| `vonUpdated→` |                                                                 `onUpdated(() => {})`                                                                 |
|   `vprops→`   |                                                     `const props = defineProps({ foo: String })`                                                      |
|   `vemits→`   |                                                      `const emit = defineEmits(['...', '...'])`                                                       |

### vue-template

|       关键词        |              代码片段               |
| :-----------------: | :---------------------------------: |
|      `vText→`       |           `v-text="..."`            |
|      `vHtml→`       |           `v-html="..."`            |
|      `vShow→`       |           `v-show="..."`            |
|       `vIf→`        |            `v-if="..."`             |
|      `velse→`       |              `v-else`               |
|     `velseif→`      |          `v-else-if="..."`          |
|       `vFor→`       |   `v-for="... in ..." :key="..."`   |
| `vFor(withoutKey)→` |        `v-for="... in ..."`         |
|       `vOn→`        |            `v-on="..."`             |
|      `vBind→`       |           `v-bind="..."`            |
|      `vModel→`      |           `v-model="..."`           |
|      `vSlot→`       |           `v-slot="..."`            |
|      `vOnce→`       |              `v-once`               |
|   `iscomponent→`    | `<component :is="..."></component>` |

### vue-router

|       关键词       |                              代码片段                               |
| :----------------: | :-----------------------------------------------------------------: |
|      `vroute`      |   `{'path':...,name:...,component: () => import('...')},mate:...`   |
|       `vrte`       |  `import { useRoute } from 'vue-router' const route = useRoute()`   |
|      `vrter`       | `import { useRouter } from 'vue-router' const router = useRouter()` |
|      `vrtes`       |                           = vrte + vrter                            |
|    `beforeeach`    |            `router.beforeEach((to, from, next) =>{...}`             |
|  `beforeresolve`   |          `router.beforeResolve((to, from, next) => {...}`           |
|    `afterEach`     |               `router.afterEach((to, from) => {...}`                |
|   `beforeenter`    |                 `beforeEnter(to, from, next) {...}`                 |
| `beforeRouteEnter` |              `beforeRouteEnter(to, from, next) {...}`               |
| `beforeRouteLeave` |              `beforeRouteLeave(to, from, next) {...}`               |

### Import and export

| 关键词 | 代码片段                                                        |
| -----: | --------------------------------------------------------------- |
| `imp→` | `import fs from 'fs';`                                          |
| `imn→` | `import 'animate.css'`                                          |
| `imd→` | `import {rename} from 'fs';`                                    |
| `ime→` | `import * as localAlias from 'fs';`                             |
| `ima→` | `import { rename  as localRename } from 'fs';`                  |
| `env→` | `export const nameVariable = localVariable;`                    |
| `enf→` | `export const log = (parameter) => { console.log(parameter);};` |

### Various methods

|   关键词 | 代码片段                                       |
| -------: | ---------------------------------------------- |
|   `fre→` | `array.forEach(currentItem => {})`             |
|   `fof→` | `for(const item of object) {}`                 |
|   `fin→` | `for(const item in object) {}`                 |
|  `anfn→` | `(params) => {}`                               |
|   `nfn→` | `const add = (params) => {}`                   |
|   `dob→` | `const {rename} = fs`                          |
|   `dar→` | `const [first, second] = [1,2]`                |
|   `sti→` | `setInterval(() => {});`                       |
|   `sto→` | `setTimeout(() => {});`                        |
|  `prom→` | `return new Promise((resolve, reject) => {});` |
|  `then→` | `.then(res => {})`                             |
| `thene→` | `.then(res => {},err=>{})`                     |
| `thenc→` | `.then(res => {}).catch((err) => {});`         |
