# A Simple Popup Tip Component for Vue.js

## Installation
```
npm i -S @yanghongjun19/vue-toast
```

## Usage
In `main.js` of a Vue Project:
```javascript
import toast from '@yanghongjun19/vue-toast';
Vue.use(toast);
```

In any Vue component, you can simply use `this.$toast()` to popup a tip:
```javascript
<script>
export default {
  mounted() {
    this.$toast({
      type: 'success',
      msg: '成功'
    });
  }
}
</script>
```

## Example
```javascript
this.$toast({
  type: 'success',
  msg: '成功',
  duration: 6
});
```
