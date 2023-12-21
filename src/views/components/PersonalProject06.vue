<template>
  <div class="personal_project06">
    <section class="section" id="personal_project">
      <h2 class="title-thin text-muted">项目作品</h2>
      <div>
        <div>
          <div></div>
          <!-- used for sizing -->

          <div class="photography">
            <div class="project">
              <figure class="portfolio-figure">
                <img src="@/assets/img/dashuju/title.png" alt="" />
              </figure>
              <div class="portfolio-caption text-center">
                <div class="valign-table">
                  <div class="valign-cell">
                    <h2 class="text-upper">公安大数据实战平台</h2>
                    <p>基于公安数据采集模型的大数据研判系统，负责公安数据的管理，展示和分析。</p>
                    <!-- <a href="#pf-popup-1" class="pf-btn-view btn btn-primary">图片</a> -->
                    <a class="btn btn-primary" @click="clickEvent(59, 'dashuju')">图片</a>
                    <a href="https://dwyp.suntang.com" class="btn btn-primary" target="_blank">前往</a>
                  </div>
                </div>
              </div>
            </div>
            <!-- .pf-popup -->
          </div>
          <!-- .pf-grid-item -->

          <div class="design">
            <div class="project">
              <figure class="portfolio-figure">
                <img src="@/assets/img/guangdaoyun/title.jpg" alt="" />
              </figure>

              <div class="portfolio-caption text-center">
                <div class="valign-table">
                  <div class="valign-cell">
                    <h2 class="text-upper">广道云</h2>
                    <p>通过拖拉拽的交互方式用于民警自制表单用于问卷调查及其他数据收集的系统</p>
                    <a class="btn btn-primary" @click="clickEvent(30, 'guangdaoyun')">图片</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- .pf-grid-item -->

          <div class="photography">
            <div class="project">
              <figure class="portfolio-figure">
                <img src="@/assets/img/yujing/title.jpg" alt="" />
              </figure>

              <div class="portfolio-caption text-center">
                <div class="valign-table">
                  <div class="valign-cell">
                    <h2 class="text-upper">多维研判预警系统</h2>
                    <p>基于electron开发的电脑桌面应用，主要用于检测系统的预警反馈到电脑上通知民警</p>
                    <a class="btn btn-primary" @click="clickEvent(8, 'yujing')">图片</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- .pf-grid-item -->
        </div>
      </div>
    </section>
    <!-- .section -->
    <el-image style="max-height: 180px" v-show="false" ref="cFImg" :src="require('@/assets/img/dashuju/title.png')" :preview-src-list="previewSrcList"></el-image>
  </div>
</template>

<script>
export default {
  data() {
    return {
      previewSrcList: []
    };
  },
  methods: {
    clickEvent(totalNum, pagname) {
      this.previewSrcList = [];
      for (let i = 1; i < totalNum; i++) {
        let temp = require('@/assets/img/' + pagname + '/1 (' + i + ').jpg');
        this.previewSrcList.push(temp);
      }

      this.$nextTick(() => {
        console.log(this.previewSrcList);
        //根据ref调起el-image组件的预览功能
        this.$refs.cFImg.clickHandler();
      });
    }
  }
};
</script>

<style lang="less" scoped>
.pf-popup-media {
  background-image: url('~@/assets/img/portfolio/ibms.jpg');
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
