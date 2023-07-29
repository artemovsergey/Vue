# Технический журнал Vue
https://vuejs.org/

# Начало

```html
<!DOCTYPE html>
<html>
<head>
<title>Изучаем Vue 3</title>
<meta charset="utf-8" />
</head>
<body>
<div id="app">
    <input type="text" v-on:input="setMessage" />
    <p>{{message}}</p>
</div>
<script src="https://unpkg.com/vue@next"></script>
<script>
Vue.createApp({
  data() {
    return {
      message: 'Hello Vue 3!'
    }
  },
  methods: {
    setMessage(event) {
      this.message = event.target.value;
    }
  }
}).mount('#app');
</script>
</body>
</html>
```
