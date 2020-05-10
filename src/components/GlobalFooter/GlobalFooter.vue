<template>
  <div class="footer">
    <div class="links">
      <!--<a-->
        <!--href="http://helloblog.byteblogs.com/#/"-->
        <!--target="_blank"-->
      <!--&gt;zynzs</a>-->
      <!--<a-->
        <!--href="https://github.com/byteblogs168/hello-blog-admin"-->
        <!--target="_blank"-->
      <!--&gt;-->
        <!--<a-icon type="github" />-->
      <!--</a>-->
      <a href="https://github.com/zhangdanan">zynzs</a>
    </div>
    <div class="copyright">
      Copyright
      <a-icon type="copyright" /> 2019-{{year}} <span>一个很棒很棒的系统</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'GlobalFooter',
  data () {
    return {
      year: new Date().getFullYear()
    }
  }
}
</script>

<style lang="less" scoped>
.footer {
  padding: 0 16px;
  margin: 48px 0 24px;
  text-align: center;

  .links {
    margin-bottom: 8px;

    a {
      color: rgba(0, 0, 0, 0.45);

      &:hover {
        color: rgba(0, 0, 0, 0.65);
      }

      &:not(:last-child) {
        margin-right: 40px;
      }
    }
  }
  .copyright {
    color: rgba(0, 0, 0, 0.45);
    font-size: 14px;
  }
}
</style>
