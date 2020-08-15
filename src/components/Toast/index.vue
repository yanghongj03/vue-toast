<template>
   <div class="uco-toast" v-if="isShow">
      {{msg}}
    </div>
</template>
<script>
export default {
  data () {
    return {
      isShow: false,
      type: 'success',
      msg: '成功',
      duration: 1
    }
  },
  mounted () {
    this.isShow = true
    setTimeout(() => {
      this.isShow = false
    }, this.duration * 1000)
  }
}
</script>
<style  scoped>
.uco-toast {
    background-color: rgba(0, 0, 0, 0.5);
    width: 80px;
    color: white;
    border-radius: 15px;
    height: 30px;
    font-size: 14px;
    line-height: 30px;
    text-align: center;
    position: relative;
    z-index: 1000;
    margin-left: -40px;
    margin-top: -15px;
    left: 50%;
    top: -50%;
}
</style>
