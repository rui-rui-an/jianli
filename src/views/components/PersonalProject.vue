<template>
  <div class="personalProject">
    <section class="section brd-btm" id="personalProject">
      <h2 class="title-thin text-muted">个人项目</h2>

      <div class="row">
        <div class="col-sm-6 clear-mrg">
          <div class="award-box">
            <figure class="award-img">
              <!-- <img src="@/assets/img/my/cet6.jpg" alt="" /> -->
              <el-image @click="toProject" style="max-height: 180px" :src="require('@/assets/img/personProject/hkzf.jpg')" :preview-src-list="[require('@/assets/img/personProject/hkzf.jpg')]"></el-image>
            </figure>

            <h3 @click="toProject" class="award-title">React租房项目</h3>
          </div>
        </div>
        <!-- .col-sm-6 -->

        <!-- <div class="col-sm-6 clear-mrg">
          <div class="award-box">
            <figure class="award-img">
              <el-image style="max-height: 180px" :src="require('@/assets/img/my/cet4.jpg')" :preview-src-list="[require('@/assets/img/my/cet4.jpg')]"></el-image>
            </figure>

            <h3 class="award-title">英语四级</h3>
          </div>
        </div> -->

        <!-- <div class="col-sm-6 clear-mrg">
          <div class="award-box">
            <figure class="award-img">
              <el-image style="max-height: 180px" :src="require('@/assets/img/my/doubleDegree.jpg')" :preview-src-list="[require('@/assets/img/my/doubleDegree.jpg')]"></el-image>
            </figure>

            <h3 class="award-title">工程管理(学信网)</h3>
          </div>
        </div> -->

        <!-- <div class="col-sm-6 clear-mrg">
          <div class="award-box">
            <figure class="award-img">
              <el-image style="max-height: 180px" :src="require('@/assets/img/my/doubleDegree.jpg')" :preview-src-list="[require('@/assets/img/my/doubleDegree.jpg')]"></el-image>
            </figure>
            <h3 class="award-title">翻译(学信网)</h3>
          </div>
        </div> -->
      </div>
      <!-- .row -->
    </section>
    <!-- .section -->
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
  methods:{
    toProject(){
        window.open('http://120.76.176.237:8081')
        // window.open('http://120.76.176.237:8081','_blank','resizable=yes,width=375,height=667')
    }
  }
};
</script>

<style lang="less" scoped>
.personalProject {
    .award-title{
        cursor: pointer;
    }
}
</style>
