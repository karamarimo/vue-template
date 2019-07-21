<template>
  <div id="hideen_area">aaaa</div>
</template>

<script>
const created = function() {
  setTimeout(() => {
    console.log("hidden_area_show()呼び出します")
    this.hidden_area_show()
  }, 3000)
}

const methods = {
  hidden_area_show: function() {
    console.log("hidden_area表示します")
    document.getElementById("hideen_area").style.display = "block"
    console.log("hidden_area表示しました")
  }
}

export default {
  created,
  methods
}
</script>

<style>
#hideen_area {
  display: none;
}
</style>