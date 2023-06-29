<template>
  <div class="certification">
    <section class="section brd-btm" id="certification">
      <h2 class="title-thin text-muted">证书一类</h2>

      <div class="row">
        <div class="col-sm-6 clear-mrg">
          <div class="award-box">
            <figure class="award-img">
              <!-- <img src="@/assets/img/my/cet6.jpg" alt="" /> -->
              <el-image
                 style="max-height: 180px"
                 :src="require('@/assets/img/my/cet6.jpg')"
                 :preview-src-list="[require('@/assets/img/my/cet6.jpg')]">
               </el-image>
            </figure>

            <h3 class="award-title">英语六级</h3>
          </div>
        </div>
        <!-- .col-sm-6 -->

        <div class="col-sm-6 clear-mrg">
          <div class="award-box">
            <figure class="award-img">
              <!-- <img src="@/assets/img/my/cet4.jpg" alt="" /> -->
              <el-image
                 style="max-height: 180px"
                 :src="require('@/assets/img/my/cet4.jpg')"
                 :preview-src-list="[require('@/assets/img/my/cet4.jpg')]">
               </el-image>
            </figure>

            <h3 class="award-title">英语四级</h3>
          </div>
        </div>
        <div class="col-sm-6 clear-mrg">
          <div class="award-box">
            <figure class="award-img">
              <!-- <img src="@/assets/img/my/doubleDegree.jpg" alt="" /> -->
              <el-image
                 style="max-height: 180px"
                 :src="require('@/assets/img/my/doubleDegree.jpg')"
                 :preview-src-list="[require('@/assets/img/my/doubleDegree.jpg')]">
               </el-image>
            </figure>

            <h3 class="award-title">工程管理(学信网)</h3>
          </div>
        </div>
        <div class="col-sm-6 clear-mrg">
          <div class="award-box">
            <figure class="award-img">
              <!-- <img src="@/assets/img/my/doubleDegree.jpg" alt="" /> -->
              <el-image
                 style="max-height: 180px"
                 :src="require('@/assets/img/my/doubleDegree.jpg')"
                 :preview-src-list="[require('@/assets/img/my/doubleDegree.jpg')]">
               </el-image>
            </figure>

            <h3 class="award-title">翻译(学信网)</h3>
          </div>
        </div>
      </div>
      <!-- .row -->
    </section>
    <!-- .section -->
  </div>
</template>
<script>
export default{
  data(){
    return {
    }
  }
}
</script>

<style lang="less" scoped>
.certification {
}
</style>
