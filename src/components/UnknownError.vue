<template>
  <div class="darkness">
    <div class="error_popup">
      <a href="#">
        <div class="close">
          <div class="close_rectangle1"></div>
          <div class="close_rectangle2"></div>
        </div>
      </a>

      <div class="sign_attention">

        <div class="sign_ellipse">
          <svg width="17" height="52" viewBox="0 0 17 52" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M0.032738 8.78817L3.54114 46.9826C3.74584 49.231 5.62247 51.0841 8.06819 51.2875C10.8076 51.5153 13.2224 49.5876 13.4614 46.9826L16.9698 8.78817C17.0076 8.3418 17.0124 7.84159 16.9698 7.38142C16.5614 2.93338 12.4389 -0.356861 7.76187 0.0310651C3.08481 0.419912 -0.375688 4.34105 0.032738 8.78817Z" fill="#E52352"/>
          </svg>
        </div>

        <div class="sign_dot">
          <svg width="15" height="14" viewBox="0 0 15 14" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M7.50391 13.9982C11.3792 13.9982 14.5207 11.0108 14.5207 7.32567C14.5207 3.64054 11.3792 0.653152 7.50391 0.653152C3.62863 0.653152 0.487105 3.64054 0.487105 7.32567C0.487105 11.0108 3.62863 13.9982 7.50391 13.9982Z" fill="#E52352"/>
          </svg>
        </div>
      </div>

      <div class="text_error">
        Неизвестная ошибка <!-- лучше потом переделать в p? -->
      </div>

      <div class="text_callback">
        Для более точной информации <a class="text_link" href="#">свяжитесь с нами</a>
      </div>

    </div>
  </div>

</template>

<script>
export default {
name: "UnknownError"
}
</script>

<style scoped>
  .darkness {
    position: absolute;
    width: 1922px;
    height: 994px;
    left: 0px;
    top: 86px;
    background: rgba(25, 28, 36, 0.8);
  }

  .error_popup {
    position: absolute;
    width: 403px;
    height: 294px;
    /*margin-left: auto;
    margin-right: auto;*/
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    margin: auto;
    border-radius: 10px;
    background: #FFFFFF;

    filter: drop-shadow(0px 0px 7px rgba(0, 0, 0, 0.3));
  }

  .close {
    position: absolute;
    left: 89.83%;
    right: 6.01%;
    top: 8.16%;
    bottom: 86.13%;
  }

  .close_rectangle1 {
    position: absolute;
    width: 21.93px;
    height: 1.77px;
    /*right: 17.81px;
    top: 24px;*/
    right: -3px;
    bottom: 7.5px;

    background: #E32368;
    transform: rotate(45deg);
  }

  .close_rectangle2 {
    position: absolute;
    width: 21.93px;
    height: 1.77px;
    /*right: 2.3px;
    top: 25.25px;*/
    top: 7.7px;
    right: -3px;

    background: #E32368;
    transform: rotate(135deg);
  }

  .sign_attention {
    position: absolute;
    width: 131px;
    height: 131px;
    left: 136px;
    top: 41px;

    background: #F5F9FF;
    border: 5px solid #E52352;
    border-radius: 50%;
    box-sizing: border-box;
  }

  .text_error {
    position: absolute;
    width: 351px;
    height: 37px;
    left: calc(50% - 351px/2);
    top: 187px;

    font-family: "Roboto", "Arial", sans-serif;/*не подключал Roboto*/
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 36px;
    text-align: center;
    color: #E32368;
  }

  .sign_ellipse {
    position: absolute;
    left: 0%;
    right: 0%;
    /*top: 0%;
    bottom: 23.42%;*/
    top: 23.42%;
  }

  .sign_dot {
    position: absolute;
    left: 8.75%;
    right: 8.7%;
    bottom: 19.92%;
  }

  .text_callback {
    position: absolute;
    width: 363px;
    height: 30px;
    left: calc(50% - 363px/2 + 1px);
    top: 254px;

    font-family: "Roboto", "Arial", sans-serif; /* Roboto не подключен */
    font-style: normal;
    font-weight: normal;
    font-size: 14px;
    line-height: 28px;
    text-align: center;
    color: #707070;
  }

  .text_link {
    color: #707070;
  }
</style>