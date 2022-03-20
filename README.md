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

We disable multi-word-component-names to demonstrate it is supported; however, it is not recommended.

Here's the output of npm run lint:

```
» npm run lint

> vue-eslint-plugin-client@0.1.0 lint
> vue-cli-service lint


/path/to/your/project/eslint-plugin-vue-client/src/components/Marquee.vue
  2:3  error  I am a custom message  vue/no-restricted-html-elements

/path/to/your/project/eslint-plugin-vue-client/src/components/NonCompliantButton.vue
  4:5  error  Unexpected use of forbidden HTML element button  vue/no-restricted-html-elements
```
