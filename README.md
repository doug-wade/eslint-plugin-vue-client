# eslint-plugin-vue-client

Note the config for eslint-plugin-vue:

```
{
  "env": {
    "node": true
  },
  "extends": [
    "eslint:recommended",
    "plugin:vue/vue3-recommended"
  ],
  "rules": {
    "vue/no-restricted-html-elements": ["error", "button"],
    "vue/multi-word-component-names": 0
  }
}
```

Here's the expected output of npm run lint:

```
» npm run lint

> vue-eslint-plugin-client@0.1.0 lint
> vue-cli-service lint

/path/to/your/project/vue-eslint-plugin-client/src/components/NonCompliantButton.vue
  4:5  error  Unexpected use of forbidden HTML element button  vue/no-restricted-html-elements

✖ 1 problem (1 error, 0 warnings)
```

Here's the actual output of npm run lint:

```
DESKTOP-LKMEB17 workspace/eslint-plugin-vue-client ‹master› » npm run lint

> vue-eslint-plugin-client@0.1.0 lint
> vue-cli-service lint


/home/doug/workspace/eslint-plugin-vue-client/src/App.vue
  6:3  error  Unexpected use of forbidden HTML element button  vue/no-restricted-html-elements

/home/doug/workspace/eslint-plugin-vue-client/src/components/NonCompliantButton.vue
  4:5  error  Unexpected use of forbidden HTML element button  vue/no-restricted-html-elements

✖ 2 problems (2 errors, 0 warnings)
```
