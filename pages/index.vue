<template lang="pug">
  .index
    u-banner
    section.main
      p.content
        | 悠夏爾科技以堅實的技術研發能力，結合美觀易用的介面設計、良好的使用者體驗，
        | 揉捻出最合適的商業解決方案，為您打造出色的網站與應用軟體。
    section.introduction.introduction-website
      h2.title
        span 絕佳設計
        span 美觀細膩
      p.content
        | 洞悉使用者操作習慣，透過美觀細膩的視覺設計，與易用性高的介面動線，
        | 讓您的網站在電腦與各個行動裝置上都擁有絕佳的使用體驗。
      nuxt-link.u-btn.u-btn-white(to="#") 了解服務項目
    section.parallax.parallax-alleylife
    section.parallax.parallax-cango
    section.introduction.introduction-function
      h2.title
        span 技術實力
        span 與時俱進
      p.content
        | 持續關注最新的網路技術，建構可高度擴充的系統架構，
        | 並保持充足的維護彈性和穩定性，滿足您所需要的各種技術支援和功能需求。
      nuxt-link.u-btn.u-btn-white(to="#") 了解服務項目
    section.parallax.parallax-tainan
    section.container-fluid.no-gutters
      .row
        section.col-6.image.image-employee
        section.col-6.image.image-office
    section.introduction.introduction-backend
      h2.title
        span 管理後台
        span 也能賞心悅目
      p.content
        | 悠夏爾所開發的網站內容管理系統「BACKEND」，
        | 提供美觀、直覺易用的後台介面，就連操作後台也能賞心悅目。
      nuxt-link.u-btn.u-btn-white(to="#") 了解服務項目
    section.parallax.parallax-backend
    section.image.image-backend
    u-features
    section.introduction.introduction-backend
    section#contact.contact
      //- .background(
        data-top-bottom="background-position: 50% -100px;",
        data-bottom-top="background-position: 50% 100px;",
        data-anchor-target="#contact")
      .wrapper
        h6.title 與我們合作
        p.content 打造出色產品的任務，就交給專業的悠夏爾團隊吧
        nuxt-link.u-btn.u-btn-white(to="#") 了解服務項目
</template>

<script>
  import UBanner from '~/components/Banner'
  import UFeatures from '~/components/Features'

  export default {
    components: { UBanner, UFeatures }
  }
</script>

<style lang="scss" scoped>
  .index {
    .main {
      background-color: #fff;
      padding: 25vmin 10vmin;
      font-size: 4.5vmin;
      line-height: 8.5vmin;
      text-align: center;
    }

    .contact {
      height: 28.125rem;
      color: #fff;
      display: flex;
      flex-direction: column;
      align-content: center;
      justify-content: center;

      .wrapper {
        padding: 0 2rem;
        text-align: center;

        .title {
          font-size: 2rem;
          margin-bottom: 1rem;
        }

        .content {
          margin-bottom: 2rem;
        }
      }
    }

    .introduction {
      color: #fff;
      background-color: #262c32;
      padding: 25vmin 10vmin;

      .title {
        font-size: 11vmin;
        line-height: 14vmin;

        > * {
          display: block;
        }
      }

      .content {
        padding: 5vmin 0;
        line-height: 1.75rem;
      }
    }

    .parallax, .image {
      background-size: cover;
      background-position: center center;
      background-repeat: no-repeat;
    }

    .parallax {
      height: 50vh;

      &-alleylife {
        background-color: #efcc24;
      }

      &-cango {
        background-color: #e0e0e0;
      }

      &-tainan {
        background-color: #fd5656;
      }

      &-backend {
        background-color: #77c7c2;
      }
    }

    .image {
      &-employee, &-office {
        height: 30vh;
      }

      &-backend {
        height: 50vh;
      }
    }
  }
</style>