<script>
export default {
  data() {
    return {
      radio: '1'
    };
  }
};
</script>

## Radio组件

### 基础用法

```html
<zan-radio name="1" v-model="radio1">单选框1</zan-radio>
<zan-radio name="2" v-model="radio1">单选框2</zan-radio>

<script>
export default {
  data() {
    return {
      radio1: '1'
    }
  }
};
</script>
```

### 禁用状态

```html
<zan-radio name="1" v-model="radio2" disabled>未选中禁用</zan-radio>
<zan-radio name="2" v-model="radio2" disabled>选中且禁用</zan-radio>

<script>
export default {
  data() {
    return {
      radio2: '2'
    }
  }
};
</script>
```

### radio组

```html
<zan-radio-group v-model="radio3">
  <zan-radio name="1">单选框1</zan-radio>
  <zan-radio name="2">单选框2</zan-radio>
</zan-radio-group>

<script>
export default {
  data() {
    return {
      radio3: '1'
    }
  }
};
</script>
```

### 与Cell组件一起使用

```html
<zan-radio-group v-model="radio4">
  <zan-cell-group>
    <zan-cell><zan-radio name="1">单选框1</zan-radio></zan-cell>
    <zan-cell><zan-radio name="2">单选框2</zan-radio></zan-cell>
  </zan-cell-group>
</zan-radio-group>

<script>
export default {
  data() {
    return {
      radio4: '1'
    }
  }
};
</script>
```

### Radio API

| 参数       | 说明      | 类型       | 默认值       | 可选值       |
|-----------|-----------|-----------|-------------|-------------|
| disabled | 是否禁用单选框 | Boolean  | false |   |
| name | 根据这个来判断radio是否选中 | Boolean  | false |   |

### RadioGroup API

| 参数       | 说明      | 类型       | 默认值       | 可选值       |
|-----------|-----------|-----------|-------------|-------------|
| disabled | 是否禁用单选框 | Boolean  | false |   |