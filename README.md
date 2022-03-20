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

```
» npm run lint

> vue-eslint-plugin-client@0.1.0 lint
> vue-cli-service lint

/path/to/your/project/vue-eslint-plugin-client/src/components/NonCompliantButton.vue
  4:5  error  Unexpected use of forbidden HTML element button  vue/no-restricted-html-elements

✖ 1 problem (1 error, 0 warnings)
```
