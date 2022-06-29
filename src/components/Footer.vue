<template>
  <section>
    <div class="copyright">
      <p>
        <a href="https://vuejs.org/">WEBSITE BUILT WITH VUEJS.ORG.</a>
      </p>
    </div>
  </section>
</template>

<script>

export default {
  name: "MyFooter",

  data() {
    return {
     
    };
  },
};
</script>

<style lang="scss" scoped>
.footer-wrap {
  padding: 40px 0 0;
  background-color: #000;

  .footer-content {
    width: 70%;
    max-width: 1170px;
    margin: 0 auto;
    display: flex;
    color: #fff;

    @media (max-width: 992px) {
      width: 95%;
    }

    @media (max-width: 750px) {
      width: 70%;
      display: block;
    }

    .item {
      width: 32%;
      margin: 0 15px 20px;

      @media (max-width: 750px) {
        width: 100%;
        margin: 0 0 20px;
      }

      .image {
        overflow: hidden;
        width: 100%;

        img {
          object-fit: cover;
          width: 100%;
          max-height: 130px;
        }
      }
    }

    .title {
      background-color: #ececec;
      font-size: 13px;
      padding: 12px;
      color: #000;
      margin: 0 0 30px;
      font-weight: unset;
      text-align: center;
      word-wrap: break-word;
      position: relative;
      user-select: none;

      &::before {
        content: "";
        left: calc(50% - 5px);
        position: absolute;
        border: 10px solid;
        border-color: #ececec transparent transparent transparent;
        top: calc(100%);
      }
      @media (min-width: 800px) {
        font-size: 18px;
      }
    }

    .list-tags {
      display: flex;
      flex-wrap: wrap;

      .tag {
        border: 1px solid #fff;
        color: #fff;
        text-decoration: none;
        font-size: 14px;
        padding: 2px 7px;
        margin: 0 10px 10px 0;
        transition: 0.6s all linear;

        &:hover {
          border: 1px solid #fff;
          background-color: #fff;
          color: #000;
        }
      }
    }

    .subcribe-info {
      padding: 0 15px 25px;
      background-color: #000;
      color: #fff;
      text-align: center;

      p {
        margin-bottom: 24px;
      }

      input {
        display: block;
        padding: 5px 10px;
        margin: 0 auto;
        border-radius: 3px;
        transition: all .5s ease-in-out;
        border: 1px solid transparent;
        margin-bottom: 24px;
        background-color: transparent;
        color: #fff;

        &:focus {
          border: 1px solid #d3b062;
          outline: 0;
        }
      }

      .btn-subcribe {
        cursor: pointer;
        background-color: #ececec;
        padding: 10px 25px;
        color: #000;
        font-size: 12px;
        line-height: 1.5;
        text-align: center;
        border: 0;
        outline: 0;
        font-weight: 400;
        letter-spacing: 1px;
      }
    }
  }

  .socials-container {
      padding-bottom: 30px;
      text-align: center;
      border-bottom: 1px solid #fff;

      .menu-socials {
        display: flex;
        justify-content: center;

        .menu-item {
          padding: 0 40px;

          .twitter, .instagram, .youtube {
            cursor: pointer;
            width: auto;
            height: 25px;
            color: #fff;

            &:hover  {
              transform: scale(1.1);
            }
          }
        }
      }
    }

  .copyright {
    text-align: center;
    padding: 20px 0;

    a {
      font-size: 12px;
      color: #d3b062;
      text-decoration: none;

      &:hover {
        color: #c1c1c1;
      }
    }
  }
}
</style>