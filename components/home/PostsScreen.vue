<template>
  <!-- blogs -->
  <div class="card">
    <div class="card-grid">
      <div class="title">
        <h2>最近更新的博客</h2>
        <p>人家文采并不是很好啦，(✿◡‿◡)。</p>
      </div>

      <div class="">

      </div>
      <a class="more" href="http://blog.onelong.org" target="_blank">查看我的博客</a>
    </div>
  </div>
</template>

<script>
import api from '@/api/api'
export default {
  mounted () {
    api.getPostsXml().then(res => {
      console.log(res)
    })
  }
}
</script>