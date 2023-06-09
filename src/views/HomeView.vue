<template>
  <div class="home">
    <div class="ace-wrapper">
      <header id="ace-header" class="ace-container-shift ace-logo-in ace-head-boxed ace-nav-right">
        <div class="ace-head-inner"></div>
      </header>
      <article id="ace-card" class="ace-card bg-primary">
        <div class="ace-card-inner text-center">
          <img class="avatar avatar-195" src="@/assets/img/my/me.jpg" width="195" height="195" alt="" />
          <h1>廖睿</h1>
          <p class="text-muted">深圳 | 广道 | 前端开发工程师</p>
          <ul class="ace-social clear-list">
            <li>
              <a :href="site.github" :title="site.github" target="_blank"><span class="ace-icon ace-icon-github"></span></a>
            </li>
            <li>
              <a :href="site.facebook" :title="site.facebook" target="_blank"><span class="ace-icon ace-icon-facebook"></span></a>
            </li>
            <li>
              <a title="15979058318"><span class="ace-icon ace-icon-phone"></span></a>
            </li>
            <li>
              <a :href="site.email" title="site.email"><span class="ace-icon ace-icon-contact"></span></a>
            </li>
          </ul>
        </div>
        <footer class="ace-card-footer">
          <a class="btn btn-lg btn-block btn-thin btn-upper" href="javascript:void(0)" onclick="window.print()">Download Resume</a>
        </footer>
      </article>
      <!-- 主要内容 -->
      <div id="ace-content" class="ace-container-shift">
        <div class="ace-container">
          <div id="ace-nav-wrap" class="hidden-sm hidden-xs">
            <div class="ace-nav-cont">
              <div id="ace-nav-scroll">
                <nav id="ace-nav" class="ace-nav">
                  <ul class="clear-list">
                    <li>
                      <a href="index.html" data-tooltip="Home"><img class="avatar avatar-42" src="@/assets/img/show-star.png" alt="" /></a>
                    </li>
                    <li>
                      <a href="#basic_info" data-tooltip="基本信息"><span class="ace-icon ace-icon-home"></span></a>
                    </li>
                    <li>
                      <a href="#profetional" data-tooltip="职业技能"><span class="ace-icon ace-icon-experience"></span></a>
                    </li>

                    <li>
                      <a href="#education" data-tooltip="教育经历"><span class="ace-icon ace-icon-portfolio"></span></a>
                    </li>

                    <li>
                      <a href="#experience" data-tooltip="工作经历"><span class="ace-icon ace-icon-references"></span></a>
                    </li>
                    <li>
                      <a href="#certification" data-tooltip="获得证书"><span class="ace-icon ace-icon-blog"></span></a>
                    </li>
                    <li>
                      <a href="#personal_project" data-tooltip="个人作品"><span class="ace-icon ace-icon-snowflake-o"></span></a>
                    </li>
                  </ul>
                </nav>
              </div>

              <div id="ace-nav-tools" class="hidden">
                <span class="ace-icon ace-icon-dots-three-horizontal"></span>

                <button id="ace-nav-arrow" class="clear-btn">
                  <span class="ace-icon ace-icon-chevron-thin-down"></span>
                </button>
              </div>
            </div>

            <!-- <div class="ace-nav-btm"></div> -->
          </div>
          <!-- .ace-nav-wrap -->

          <div class="ace-paper-stock">
            <main class="ace-paper clearfix">
              <div class="ace-paper-cont clear-mrg">
                <!-- START: PAGE CONTENT -->
                <div class="padd-box clear-mrg">
                  <Basic01 />
                  <Profetional02 />
                  <Education03 />
                  <Experience04 />
                  <Certification05 />
                  <PersonalProject06 />
                </div>
                <!-- .padd-box -->
                <!-- END: PAGE CONTENT -->
              </div>
              <!-- .ace-paper-cont -->
            </main>
            <!-- .ace-paper -->
          </div>
          <!-- .ace-paper-stock -->
        </div>
        <!-- .ace-container -->
      </div>
      <!-- Triangle Shapes -->
      <svg id="ace-bg-shape-1" class="hidden-sm hidden-xs" height="519" width="758">
        <polygon points="0,455,693,352,173,0,92,0,0,71" style="fill: #d2d2d2; stroke: purple; stroke-width: 0; opacity: 0.5" />
      </svg>

      <svg id="ace-bg-shape-2" class="hidden-sm hidden-xs" height="536" width="633">
        <polygon points="0,0,633,0,633,536" style="fill: #c0e3e7; stroke: purple; stroke-width: 0" />
      </svg>
    </div>
  </div>
</template>

<script>
import Basic01 from './components/Basic01.vue';
import Profetional02 from './components/Profetional02.vue';
import Education03 from './components/Education03.vue';
import Experience04 from './components/Experience04.vue';
import Certification05 from './components/Certification05.vue';
import PersonalProject06 from './components/PersonalProject06.vue';
export default {
  name: 'HomeView',
  data() {
    return {
      site: {}
    };
  },
  computed: {},
  created() {},
  methods: {},
  components: { Basic01, Profetional02, Education03, Experience04, Certification05, PersonalProject06 }
};
</script>
<style lang="less" scoped></style>
