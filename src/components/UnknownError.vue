<template>
  <div class="darkness">
    <div class="error_popup">
      <ButtonClose />
      <div class="sign_attention">
        <img class="image" src="@/assets/sign_attention.svg" alt="внимание">
        <span class="text_error">Неизвестная ошибка</span>
        <span class="text_callback">
          Для более точной информации <a class="text_link" href="#">свяжитесь с нами</a>
        </span>
      </div>
    </div>
  </div>
</template>

<script>
  import ButtonClose from "@/components/ButtonClose";
  export default {
  name: "UnknownError",
    components: {ButtonClose}
  }
</script>

<style scoped>
  .darkness {
    position: absolute;
    width: 100%;
    height: calc(100% - 5.375rem);
    top: 5.375rem;
    left: 0rem;
    background: rgba(25, 28, 36, 0.8);
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .error_popup {
    position: relative; /*для MS Edge чтобы крестик отображался внутри окошка */
    width: 25.1875rem;
    height: 18.375rem;
    border-radius: 10px;
    background: #FFFFFF;
    filter: drop-shadow(0px 0px 7px rgba(0, 0, 0, 0.3));
    display: flex;
    justify-content: center;
  }

  .sign_attention {
    margin-top: 2.5625rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  .text_error {
    font-family: "Roboto", "Arial", sans-serif;/*не подключал Roboto*/
    font-style: normal;
    font-weight: 500;
    font-size: 1.25rem;
    text-align: center;
    color: #E32368;
  }

  .text_callback {
    margin-bottom: 1.25rem;
    font-family: "Roboto", "Arial", sans-serif; /* Roboto не подключен */
    font-style: normal;
    font-weight: normal;
    font-size: 0.875rem;
    text-align: center;
    color: #707070;
  }

  .text_link {
    color: #707070;
  }

  .image { /* Нужно чтобы правильно отобразился размер картинки в MS Edge */
    height: 8.1875rem;
  }
</style>