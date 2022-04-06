<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <!--
          <li>
            <a href="https://www.creative-tim.com">
              Creative Tim
            </a>
          </li>
          -->
          <li>
            <a href="">
              关于我们
            </a>
          </li>
          <li>
            <a href="https://encoderlee.blog.csdn.net/">
              博客
            </a>
          </li>
          <!--
          <li>
            <a href="https://www.creative-tim.com/license">
              Licenses
            </a>
          </li>
          -->
        </ul>
      </nav>
      <div class="copyright">
        <p>开发元宇宙链游自动化脚本服务<br />版权所有 &copy; {{ year }}</p>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
