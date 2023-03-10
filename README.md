# FE-cheat-sheet

## cocos creator 源码
1. [消除](https://github.com/CoderLim/pop_stars)
2. [简版消消乐](https://gitee.com/coder-lim/simple-xiaoxiaole)
3. [炮弹抛射](https://gitee.com/coder-lim/cocos-case-projectile)
4. [2048](https://gitee.com/coder-lim/cocos-creator3.x-2048)
5. [一堆效果](https://gitee.com/coder-lim/cocos-creator-examples)

## 开发技巧
1. cmd+\ 或 F8 可以立即断下来，方便查看 popover 的样式；

## VSCode
### 插件
AutoCloseTag
AutoCompleteTag
AutoRenameTag
CodeSpellChecker
ESLint
StyleLint
GitGraph
importCost
Prettier - Code formatter
Tailwind CSS IntelliSense
TODO Highlight
Vetur
Vim
ChatGPT

### 配置
```
// .vscode/extensions.json
{
  "recommendations": [
    "editorconfig.editorconfig",
    "dbaeumer.vscode-eslint",
    "jpoissonnier.vscode-styled-components",
    "drknoxy.eslint-disable-snippets",
    "wix.vscode-import-cost",
    "eg2.vscode-npm-script",
    "wayou.vscode-todo-highlight",
    "esbenp.prettier-vscode"
  ]
}

```

```
// .vscode/settings.json
{
  "typescript.tsdk": "node_modules/typescript/lib",
  "eslint.options": {
    "configFile": "./.eslintrc"
  },
  "eslint.probe": ["javascript", "javascriptreact", "typescript", "typescriptreact", "html", "vue", "markdown"],
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
    // "source.organizeImports": true
  },
  "editor.formatOnSave": true,
  "autoimport.useSemiColon": true,
  "[json]": {
    "editor.tabSize": 2,
    "editor.formatOnType": true,
    "editor.formatOnPaste": true,
    "editor.formatOnSave": true
  },
  "[jsonc]": {
    "editor.tabSize": 2,
    "editor.formatOnType": true,
    "editor.formatOnPaste": true,
    "editor.formatOnSave": true
  },
  "cSpell.words": ["aksks", "unavail"],
  "typescript.format.insertSpaceAfterOpeningAndBeforeClosingEmptyBraces": true
}
```

```
// .prettierrc
{
  "printWidth": 120,
  "tabWidth": 2,
  "trailingComma": "all",
  "jsxBracketSameLine": true,
  "semi": true,
  "singleQuote": true,
  "arrowParens": "avoid",
  "overrides": [
    {
      "files": "*.ts",
      "options": {
        "parser": "typescript"
      }
    }
  ]
}
```

```
// .stylelintrc.json
{
  "extends": "stylelint-config-recommended",
  "rules": {
    "no-descending-specificity": null,
    "declaration-colon-newline-after": null,
    "at-rule-no-unknown": null,
    "selector-pseudo-class-no-unknown": [
      true,
      {
        "ignorePseudoClasses": ["global"]
      }
    ]
  }
}

```

```
.eslintrc
{
  "root": true,
  "env": {
    "browser": true,
    "es6": true
  },
  "extends": ["eslint:recommended", "plugin:react/recommended", "plugin:@typescript-eslint/recommended"],
  "parser": "@typescript-eslint/parser",
  "parserOptions": {
    "ecmaFeatures": {
      "experimentalObjectRestSpread": true,
      "jsx": true
    },
    "sourceType": "module"
  },
  "plugins": ["@typescript-eslint", "react", "react-hooks"],
  "settings": {
    "react": {
      "version": "detect"
    }
  },
  "rules": {
    // "indent": ["error", 2, { "SwitchCase": 1 }],
    "quotes": ["error", "single"],
    "semi": ["error", "always"],
    "no-console": "error",
    "block-spacing": ["error", "always"],
    "no-trailing-spaces": "error",
    "object-curly-spacing": ["error", "always"],
    "no-empty": 0,
    "react/prop-types": [
      "warn",
      {
        "ignore": ["children"]
      }
    ],
    "@typescript-eslint/no-unused-vars": ["warn", { "vars": "local" }],
    "@typescript-eslint/ban-ts-ignore": 0,
    "@typescript-eslint/ban-ts-comment": 0,
    "@typescript-eslint/no-explicit-any": 0,
    "@typescript-eslint/camelcase": 0,
    "@typescript-eslint/no-empty-interface": 0,
    "@typescript-eslint/explicit-function-return-type": 0,
    "@typescript-eslint/no-non-null-assertion": 0,
    "@typescript-eslint/explicit-module-boundary-types": 0,
    "arrow-parens": [2, "as-needed"]
  }
}

```

## HTML

1. [一张图搞定各种属性：offsetTop、clientTop、scrollTop等](https://www.programering.com/a/MTM2QTNwATA.html)
## CSS

1. [BEM common problems](https://www.w3cplus.com/css/battling-bem-extended-edition-common-problems-and-how-to-avoid-them.html)

## React

1. [react 揭秘](https://react.iamkasong.com/)
2. [Build your react](https://pomb.us/build-your-own-react/)
3. [Build your own x](https://github.com/danistefanovic/build-your-own-x)
4. [react-philosophies](https://github.com/mithi/react-philosophies)

## GIT
1. [图解 GIT](https://marklodato.github.io/visual-git-guide/index-zh-cn.html)
2. [这才是真正的Git——Git内部原理揭秘！](https://zhuanlan.zhihu.com/p/96631135)

## API

1. [10-best-practices-for-writing-node-js-rest-apis](https://blog.risingstack.com/10-best-practices-for-writing-node-js-rest-apis/)

## Design Pattern

1. [工厂模式，依赖注入](https://medium.com/@pyrolistical/factory-functions-pattern-in-depth-356d14801c91)

## Deploy

1. [docker化webapp](https://itnext.io/dockerizing-modern-web-apps-cd9667eebf44)

## Security

1. [helmet.js](https://helmetjs.github.io/)
2. [Auth2.0](https://www.chrisyue.com/security-issue-about-oauth-2-0-you-should-know.html)
   [Auth2.0 RFC](https://tools.ietf.org/html/rfc6749#section-4.2)
## Node

1. [node定时器详解](http://www.ruanyifeng.com/blog/2018/02/node-event-loop.html)
2. [nodejs-->timer](https://alinode.aliyun.com/blog/9)
3. [写一个脚手架](https://juejin.cn/post/6932610749906812935?utm_source=gold_browser_extension)

## TDD

1. [https://blog.risingstack.com/getting-node-js-testing-and-tdd-right-node-js-at-scale/](https://blog.risingstack.com/getting-node-js-testing-and-tdd-right-node-js-at-scale/)

## Browser 

1. [浏览器多进程到JS单线程](https://juejin.im/post/5a6547d0f265da3e283a1df7)
2. [js编译器结构、Shape、IC、对象和数组是如何存储的](https://mathiasbynens.be/notes/shapes-ics)
3. [Tasks, microtasks, queues and schedules](https://jakearchibald.com/2015/tasks-microtasks-queues-and-schedules/)

## 函数式编程

1. [很不错的gitbook](https://llh911001.gitbooks.io/mostly-adequate-guide-chinese/content/ch1.html)

## Better

1. [https://www.coderhood.com/5-problem-solving-skills-great-software-developers/](https://www.coderhood.com/5-problem-solving-skills-great-software-developers/)
2. [How to read es specification](https://timothygu.me/es-howto/)
3. [组件库的思考](https://github.com/fex-team/fit/issues/3)
4. [Cam Jackson: 微前端](https://martinfowler.com/articles/micro-frontends.html)

## ML

1. [入门必备](https://github.com/KeKe-Li/tutorial)
2. [谷歌教程](https://developers.google.com/machine-learning/crash-course/)
3. [Tensorflow：识别手写数字](https://gitbook.cn/gitchat/column/59f7e38160c9361563ebea95#catalog)

## 成品
1. [HooksAdmin react 管理后台](https://github.com/HalseySpicy/Hooks-Admin)
2. [Geeker vue 管理后台](https://github.com/HalseySpicy/Geeker-Admin)

## QA

1. [为什么 inline-block 且 overflow:hidden 的元素的 baseline 在元素底部](https://stackoverflow.com/questions/32078950/why-baseline-of-inline-block-element-with-overflowhidden-is-set-to-its-bott/34183059)
2. [inlineblock 的 vertical-align](https://github.com/o2team/H5Skills/issues/47)
