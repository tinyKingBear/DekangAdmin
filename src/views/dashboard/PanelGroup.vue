<template>
  <el-row :gutter="40" class="panel-group">
    <el-col :xs="12" :sm="12" :lg="12" class="card-panel-col">
      <div class="card-panel">
        <div class="title">影像数量</div>
        <div class="count-content">
          <div class="count">12,005,389张</div>
          <div class="detial">明细&nbsp;></div>
        </div>
      </div>
    </el-col>
    <el-col :xs="12" :sm="12" :lg="12" class="card-panel-col">
      <div class="card-panel bg-color">
        <div class="title">调阅数量</div>
        <div class="count-content">
          <div class="count">45,345,567次</div>
          <div class="detial">明细&nbsp;></div>
        </div>
      </div>
    </el-col>
  </el-row>
</template>

<script>
export default {
  data() {
    return {
      count: { newIp: 0, newVisits: 0, recentIp: 0, recentVisits: 0 }
    }
  },
  mounted() {
  }
}
</script>

<style rel="stylesheet/scss" lang="scss" scoped>
.panel-group {
  margin-top: 18px;
  .card-panel-col{
    margin-bottom: 32px;
  }
  .bg-color {
    background: #7d85fa !important;
  }
  .card-panel {
    height: 108px;
    font-size: 16px;
    position: relative;
    overflow: hidden;
    color: white;
    background: #3c85fd;
    box-shadow: 4px 4px 40px rgba(0, 0, 0, .05);
    border-color: rgba(0, 0, 0, .05);
    border-radius: 10px;
    padding: 20px 15px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    .title {
      color: white;
      font-size: 20px;
      font-weight: bold;
      letter-spacing: 3px;
    }
    .count-content {
      display: flex;
      align-items: center;
      justify-content: space-between;
      .count {
        font-size: 20px;
      }
      .detail {
        font-size: 16px;
      }
    }
  }
}
</style>
