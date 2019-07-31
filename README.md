# vue-at-hook

```html
<!-- Parent.vue -->
<template>
  <div class="parent">
    <Child @hook:mounted="childMounted" />
  </div>
</template>

<script>
export default {
  name: "Parent",
  methods: {
    childMounted() {
      console.log(`childMounted`)
    }
  }
}
</script>
```

```html
<!-- Child.vue -->
<template>
  <div class="child">
  </div>
</template>

<script>
export default {
  name: "Child"
}
</script>
```

https://github.com/MonguDykrai/vue-at-hook.git